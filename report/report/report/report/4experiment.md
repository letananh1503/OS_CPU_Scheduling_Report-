def print_gantt_chart(processes):
    print("\nGantt Chart:")

    print(" ", end="")
    for p in processes:
        print("-------", end="")
    print()

    print("|", end="")
    for p in processes:
        print(f"  {p.name:^3}  |", end="")
    print()

    print(" ", end="")
    for p in processes:
        print("-------", end="")
    print()

    print(processes[0].start_time, end="")
    for p in processes:
        print(f"{p.completion_time:>7}", end="")
    print()

