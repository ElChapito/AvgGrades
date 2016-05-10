int[] tableSort(int[] array){
		int[] tally = new int[1001];
		for (int i = 0; i < array.length; i++) {
			tally[array[i]]++;
		}
		//i keeps track of actual number
		int count = 0;
		for (int i = 0; i < tally.length; i++) {
			//j keeps track of how many times we've seen that number
			for (int j = 0; j < tally[i]; j++) {
				array[count] = i;
				count++;
				
			}
			
		}
		
		return array;
	}


