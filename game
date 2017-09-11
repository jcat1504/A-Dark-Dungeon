def start
  puts "You awaken from a slumber for God knows how long."
  puts "You walk outside to find that you were sleeping in the Room of Light."
  puts "You pick up a sword and shield and proceeded to the next room."
  ground_floor
end

  def ground_floor
    puts "This room is completely barren."
    puts "Suddenly! An enemy appears. Looks like an undead coyote."
    puts "Attack or defend?"
    print "> "
    choice = $stdin.gets.chomp

    if choice.include? "attack"
      puts "Great! You got him."
      decisions
    elsif choice.include? "defend"
      puts "You blocked him and attacked. He died."
      decisions
    else
      ground_floor
    end
  end

  def decisions
    puts "You have three rooms ahead of you. Choose wisely."
    puts "1. Despair "
    puts "2. Deceit "
    puts "3. Filth "
    print "> "
    choice = $stdin.gets.chomp

    if choice == "1"
      despair_room
    elsif choice == "2"
        deceit_room
      else choice == "3"
        filth_room
    end
  end

  def despair_room
    puts "There is a huge bat monster..."
    puts "It glares at you. What do you do?"
    puts "Attack"
    puts "Flee"
    bat_attack = false

    while true
      print "> "
      choice = $stdin.gets.chomp
      if choice == "attack"
        puts "You attacked! But  he isn't dead yet..."
        bat2
      elsif choice == "flee" || bat_attack
        puts "You fled back to previous room. "
        decisions
      else
        die("Too bad!")
      end
    end
end

def bat2
  puts "Attack again or shield his next move?"
  print "> "
  choice = $stdin.gets.chomp

  if choice == "attack"
    die("He got you first!")
  elsif choice == "shield"
    puts "You dodged his attack and hit him twice! Onto the next room."
    upstairs
  else
    die("You stumbled around and tripped.")
end
end

def upstairs
  puts "You see a stairway and proceeded."
  puts "> "
  puts "> "
  puts "> "
  elements_room
end

def deceit_room
  puts "You walk around to find that it is completely dark."
  puts "You find a torch and a switch next to it..."
  puts "Do you turn on the switch? Yes or no?"
  print "> "
  choice = $stdin.gets.chomp
  if choice == "yes"
    puts "You hear a door unlock somewhere and proceeded onward."
    solitude_room
  elsif choice == "no"
    puts "Try again."
    deceit_room
  else
    start
  end
end

def filth_room
  puts "You find yourself in a crowded room..."
  puts "Except it's not crowded with people But with bats and slime monsters."
  puts "What do you do?"
  puts "1. Run or 2. Fight?"
  print "> "
  choice = $stdin.gets.chomp
  if choice == "1"
    die("You run to the nearest room but it's locked!")
  elsif choice == "2"
    puts "So you fight the monsters. A slime dropped a key..."
    puts "You opened the door to the next room."
    rage_room
  else
    die("You slipped!")
  end
end

def rage_room
  puts "You enter the room and it is completely dark..."
  puts "You hear a ticking sound in the darkness."
  sounds = []
(0..5). each do |i|
  puts " #{i}"
end

  noise = ['I''m', 'coming', 'for', 'you']
  noise.each do |noise|
  puts " #{noise}"
end

  puts "What do you do?!"
  puts "Flee or attack?"
  print "> "
  choice = $stdin.gets.chomp

  if choice == "flee"
    puts "Close call! You grabbed a nearby torch and proceeded to the next room."
    chamber
  elsif choice == "attack"
      die("The demon reveals itself and possesses you.")
    end
  end


def chamber
  puts "You enter a room with a stone slab in the center."
  puts "It has words printed on it..."
  sin = ['It', 'Does', 'Not', 'Falter.']
  sin.each do |sin|
    puts " #{sin}"
  end
  puts "Death is a part of this world and will renew its cycle."
  puts "They call it Sin."
  puts "You proceeded onwards..."
  upstairs
#room of elements
end

def solitude_room
  puts "This room is completely barren."
  puts "You walk towards the center to find a big stone slab."
  puts "There seems to be some writing printed."
  print "..."
  puts "There are elements in this world:"
unknown = ['Fire', 'Ice', 'Wind', 'Water']
unknown.each do |elements|
  puts "#{elements}"
end
  puts "We need these elements to maintain balance into this world."
  upstairs
  elements_room
end

def elements_room
  puts "You walk into a brightly lit room..."
  puts "You walk towards a door that reads:"
  puts "Collect 20 elemental orbs to proceed."
  puts "You look around and collected some element orbs."
  elements
end

def elements
  orb = "5"
  puts "You collected #{orb} fire orbs, #{orb} ice orbs, #{orb} wind orbs, #{orb} water orbs."
puts "You inserted each orb into the door and it starts to open slowly..."
puts "> "
puts "> "
puts "> "
puts "You made it back to the outside world. Yay!"
exit(0)
end



  def die(why)
    puts why, "You died. Game over."
    exit(0)
  end


start
