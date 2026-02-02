def print_gantt_chart(processes):
    print("\nGantt Chart:")

    # Dòng trên
    print(" ", end="")
    for p in processes:
        print("-------", end="")
    print()

    # Dòng tên process
    print("|", end="")
    for p in processes:
        print(f"  {p.name:^3}  |", end="")
    print()

    # Dòng dưới
    print(" ", end="")
    for p in processes:
        print("-------", end="")
    print()

    # Dòng thời gian
    print(processes[0].start_time, end="")
    for p in processes:
        print(f"{p.completion_time:>7}", end="")
    print()

