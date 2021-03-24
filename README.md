# goscraper
Package to quickly return a preview of a webpage, you can get easily its title, description & images

## Usage
    func main() {
		s, err := goscraper.Scrape("https://www.w3.org/", 5)
		if err != nil {
			fmt.Println(err)
			return
		}
		fmt.Printf("Icon : %s\n", s.Preview.Icon)
		fmt.Printf("Name : %s\n", s.Preview.Name)
		fmt.Printf("Title : %s\n", s.Preview.Title)
		fmt.Printf("Description : %s\n", s.Preview.Description)
		fmt.Printf("Image: %s\n", s.Preview.Images[0])
		fmt.Printf("Url : %s\n", s.Preview.Link)
	}

## License
Goscraper is licensed under the [MIT License](./LICENSE).
