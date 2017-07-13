<span data-ttu-id="a59b9-p103">Элементы DriveItem, возвращенные действием **sharedWithMe**, будут всегда содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что это элементы с другого диска. Чтобы получить доступ к общему ресурсу DriveItem, следует отправить запрос, используя указанные в **remoteItem** данные, в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="a59b9-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

Элементы DriveItem, возвращенные действием **sharedWithMe**, будут всегда содержать аспект [**remoteItem**](../resources/remoteitem.md), который указывает, что это элементы с другого диска. Чтобы получить доступ к общему ресурсу DriveItem, следует отправить запрос, используя указанные в **remoteItem** данные, в следующем формате:

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
