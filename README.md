# USS Commander - Submarine Warfare Simulator

A deep submarine warfare simulator that teaches real strategic thinking and decision making. Built as a single HTML file with no external dependencies.

## Game Features

### Realistic Radar System
- Authentic sonar sweep animation with CRT display effects
- Distinguishable contact types (fishing boats, submarines, airplanes)
- Visual trails showing vessel movement patterns
- Range filtering and depth control systems

### Strategic Combat System
- **Torpedoes**: Visible projectiles that travel across screen with trails
- **Enemy AI**: Hostile subs maintain optimal combat range and fire torpedoes when aligned
- **Damage Feedback**: Screen shake, red flash overlay, 3-second freeze on hit
- **Oil Trails**: Damaged ships leave visible traces for tracking

### Resource Management
- **Fuel/Reactor Output**: Affects speed and maneuverability
- **Munitions**: Limited torpedoes requiring careful targeting
- **Crew Status**: Operations capacity affected by damage
- **Supplies**: Food/oxygen for crew, degradation affects performance

### Second-Order Effects
- Firing reveals player position (acoustic signature)
- Misses create noise that masks real contacts temporarily
- Damaged ships leave oil trails visible on sonar
- Low supplies degrade equipment reliability
- Crew fatigue affects combat effectiveness

## How to Play

1. **Start the Game**: Open `index.html` in any modern web browser
2. **Understand Your Controls**:
   - Mouse click: Fire torpedoes at selected bearing
   - Keyboard 'F': Quick fire command
   - Depth slider: Filter contacts by depth
   - Range slider: Set minimum detection range

3. **Make Strategic Decisions**:
   - Classify contacts before firing (fishing vs hostile)
   - Manage resources carefully (torpedoes are limited)
   - Watch for enemy torpedoes and avoid them
   - Return to "Resupply Zone" (center area) when needed

4. **Win Condition**: Destroy all hostile submarines while maintaining crew and resources.

## Contact Types

| Type | Symbol | Behavior | Threat Level |
|------|--------|----------|-------------|
| Fishing Boat | □ | Slow, shallow, predictable movement | None - Civilian vessel |
| Hostile Submarine | ● | Fast, deep, attacks player | High - Primary target |
| Friendly Submarine | ▲ | Moves independently, avoids combat | None - Don't shoot! |
| Airplane | ▼ | Very fast, overwater only | Low - Not a threat |

## Controls

- **Mouse**: Move cursor to aim, click to fire
- **Keyboard**:
  - `F`: Fire torpedo
  - `S`: Toggle sonar active/passive
  - `G`: Toggle ghost echoes
  - `T`: Toggle contact trails
  - `R`: Resupply at base (if in zone)
  - `1-8`: Select torpedo tubes

## Game Mechanics Explained

### Resource System
Resources deplete continuously:
- Fuel: Powers reactor, affects speed
- Munitions: Limited torpedoes (8 starting)
- Crew: Operations capacity
- Supplies: Food/oxygen for crew

**Low Resources Consequences**:
- <50% fuel: Reduced reactor output
- <30% supplies: Crew fatigue increases
- <3 crew: Game over condition

### Combat Mechanics
1. **Firing**: Creates acoustic signature, masking real contacts for 3 seconds
2. **Enemy Response**: Hostile subs fire when bearing aligned and in range
3. **Damage**: Screen shake, resource loss, potential game over
4. **Oil Trails**: Damaged ships leave traces visible on sonar

### AI Behavior
- **Fishing Boats**: Wander near center, panic if approached
- **Hostile Subs**: Maintain 80-150nm range, fire when aligned with player
- **Friendly Subs**: Avoid combat, move independently

## Development Notes

Built as a single HTML file for portability and ease of testing. No external frameworks or libraries required.

### Key Technologies
- HTML5 Canvas for rendering
- Vanilla JavaScript for game logic
- Web Audio API for sonar effects
- CSS3 animations for CRT display effects

### Future Enhancements
- Multiplayer support
- Campaign mode with missions
- Advanced AI behaviors (convoy tactics)
- Submarine customization
- More contact types and scenarios

## License

MIT License - Feel free to use and modify as you see fit.

---

**Created for young naval commanders everywhere. May your strategies be brilliant and your torpedoes true! 🌊⚓**
