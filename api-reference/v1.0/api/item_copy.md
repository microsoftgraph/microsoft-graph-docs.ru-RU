# <a name="copy-a-driveitem"></a><span data-ttu-id="539eb-101">Копирование ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="539eb-101">Copy a DriveItem</span></span>

<span data-ttu-id="539eb-102">Создает копию ресурса [driveItem](../resources/driveitem.md) (включая дочерние элементы) в родительском элементе или с новым именем.</span><span class="sxs-lookup"><span data-stu-id="539eb-102">Creates a copy of a [driveItem](../resources/driveitem.md) (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="539eb-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="539eb-103">Permissions</span></span>
<span data-ttu-id="539eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="539eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="539eb-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="539eb-106">Permission type</span></span>      | <span data-ttu-id="539eb-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="539eb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="539eb-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="539eb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="539eb-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539eb-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="539eb-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="539eb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="539eb-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539eb-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="539eb-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="539eb-112">Application</span></span> | <span data-ttu-id="539eb-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="539eb-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="539eb-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="539eb-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a><span data-ttu-id="539eb-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="539eb-115">Request body</span></span>
<span data-ttu-id="539eb-116">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="539eb-116">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="539eb-117">Имя</span><span class="sxs-lookup"><span data-stu-id="539eb-117">Name</span></span>            | <span data-ttu-id="539eb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="539eb-118">Value</span></span>                                          | <span data-ttu-id="539eb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="539eb-119">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="539eb-120">parentReference</span><span class="sxs-lookup"><span data-stu-id="539eb-120">parentReference</span></span> | [<span data-ttu-id="539eb-121">ItemReference</span><span class="sxs-lookup"><span data-stu-id="539eb-121">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="539eb-p102">Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.</span><span class="sxs-lookup"><span data-stu-id="539eb-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="539eb-124">name</span><span class="sxs-lookup"><span data-stu-id="539eb-124">name</span></span>            | <span data-ttu-id="539eb-125">string</span><span class="sxs-lookup"><span data-stu-id="539eb-125">string</span></span>                                         | <span data-ttu-id="539eb-p103">Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="539eb-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="539eb-p104">**Примечание.** Свойство _parentReference_ должно включать либо `id`, либо `path`. Если включены оба элемента, они должны ссылаться на один элемент, иначе возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="539eb-p104">**Note:** The _parentReference_ should include either an `id` or `path` but not both. If both are included, they need to reference the same item or an error will occur.</span></span>

## <a name="example"></a><span data-ttu-id="539eb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="539eb-131">Example</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a><span data-ttu-id="539eb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="539eb-132">Response</span></span>

<span data-ttu-id="539eb-133">Возвращает сведения о том, как следить за процессом копирования при принятии запроса.</span><span class="sxs-lookup"><span data-stu-id="539eb-133">Returns details about how to monitor the progress of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a><span data-ttu-id="539eb-134">Заметки</span><span class="sxs-lookup"><span data-stu-id="539eb-134">Remarks</span></span>

<span data-ttu-id="539eb-p105">Во многих случаях копирование выполняется асинхронно. Отклик API указывает, что операция копирования принята или отклонена, например из-за использования имени конечного файла.</span><span class="sxs-lookup"><span data-stu-id="539eb-p105">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

<span data-ttu-id="539eb-137">**Примечание.** API не предоставляет способ, позволяющий узнать, была ли копия успешно сохранена.</span><span class="sxs-lookup"><span data-stu-id="539eb-137">**Note:** The API does not provide a method to know if the copy was successful.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
