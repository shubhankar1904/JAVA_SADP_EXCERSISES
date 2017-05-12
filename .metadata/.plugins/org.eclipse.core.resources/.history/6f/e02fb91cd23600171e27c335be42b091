package excersise1_solutions;

import java.util.ArrayList;
import java.util.stream.Collectors;
import java.util.stream.IntStream;

import excersise1.Coordinate;

public class Solutions {

	public static void main(String[] args) {
		ArrayList<Coordinate> points = new ArrayList<Coordinate>();
		points.add(new Coordinate(0, 0));
		points.add(new Coordinate(-1, 1));
		points.add(new Coordinate(-2, 4));
		points.add(new Coordinate(-2, -3));
		points.add(new Coordinate(-10, 2));
		points.add(new Coordinate(5, -1));
		points.add(new Coordinate(2, 4));
		points.add(new Coordinate(1, 0));
		points.add(new Coordinate(10, 3));
		
		System.out.println("Solution 1\n\n");
		points.forEach(System.out::println);
		
		System.out.println("\n\nSolution 2\n\n");
		points.stream()
		.mapToInt(Coordinate::getX)
		.forEach(System.out::println);
		
		System.out.println("\nSum is: " +points.stream().mapToInt(Coordinate::getX).sum());
		
		System.out.println("\n\nSolution 3\n\n");
		System.out.println("Sum of y cords :"+ points.stream()
		.mapToInt(Coordinate::getY)
		.sum()
		);
		
		System.out.println("\n\nSolution 4\n\n");
		points.stream()
		.filter(coordinate -> coordinate.getX() >= 0 )
		.filter(coordinate -> coordinate.getY() >= 0 )
		.forEach(System.out::println);
		
		System.out.println("\n\nSolution 5\n\n");
		ArrayList<Coordinate> newlist = (ArrayList<Coordinate>) points.stream()
		.filter(coordinate -> coordinate.getX() >= 0 )
		.collect(Collectors.toList());
		
		newlist.forEach(System.out::println);
	}

}
