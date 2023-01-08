import names

def get_boy_names():
    return [names.get_first_name(gender='male') for _ in range(20)]

def get_girl_names():
    return [names.get_first_name(gender='female') for _ in range(20)]

def print_names(names):
    for i, name in enumerate(names):
        print(f'{i + 1}. {name}')

def main():
    while True:
        gender = input('Enter b for boy names or g for girl names: ')
        if gender == 'b':
            names = get_boy_names()
        elif gender == 'g':
            names = get_girl_names()
        else:
            print('Invalid input. Please try again.')
            continue

        print_names(names[:10])

        while True:
            more = input('Press m for more names or c to cancel: ')
            if more == 'm':
                names = get_boy_names() if gender == 'b' else get_girl_names()
                print_names(names[:10])
            elif more == 'c':
                break
            else:
                print('Invalid input. Please try again.')

if __name__ == '__main__':
    main()
