
  public static boolean isMatch(String str) {
  
		boolean match = false;
		
		Stack<Character> stack = new Stack<>();
		
		for (int i = 0; i < str.length(); i++) {
			if (str.charAt(i) == '(' || str.charAt(i) == '{' || str.charAt(i) == '[') {
				stack.push(str.charAt(i));
			}
			else if (str.charAt(i) == ')') {
				char c = stack.pop();
				if (c == '(') {
					match = true;
				}
				else {
					match = false;
				}
			}
			else if (str.charAt(i) == '}') {
				char c = stack.pop();
				if (c == '{') {
					match = true;
				}
				else {
					match = false;
				}
			}
			else if (str.charAt(i) == ']') {
				char c = stack.pop();
				if (c == '[') {
					match = true;
				}
				else {
					match = false;
				}
			}
		} //for loop
		if (stack.empty()) {
			if (match) {
				return true;
			}
		}
		return false;
 } //method
