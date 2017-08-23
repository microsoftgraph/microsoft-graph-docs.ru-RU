# <a name="enumerate-subsites-of-a-site"></a><span data-ttu-id="6aea1-101">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="6aea1-101">Enumerate subsites of a site</span></span>

<span data-ttu-id="6aea1-102">Получение коллекции дочерних сайтов определенного [сайта][].</span><span class="sxs-lookup"><span data-stu-id="6aea1-102">Get a collection of subsites defined for a [site][].</span></span>

<span data-ttu-id="6aea1-103">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="6aea1-103">[site]: ../resources/site.md</span></span>

## <a name="permissions"></a><span data-ttu-id="6aea1-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aea1-104">Permissions</span></span>

<span data-ttu-id="6aea1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6aea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6aea1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aea1-107">Permission type</span></span>      | <span data-ttu-id="6aea1-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aea1-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6aea1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aea1-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6aea1-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aea1-110">Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6aea1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aea1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aea1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aea1-112">Not supported.</span></span>    | 
|<span data-ttu-id="6aea1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aea1-113">Application</span></span> | <span data-ttu-id="6aea1-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aea1-114">Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6aea1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aea1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{site-id}/sites
```

## <a name="example"></a><span data-ttu-id="6aea1-116">Пример</span><span class="sxs-lookup"><span data-stu-id="6aea1-116">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6aea1-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aea1-117">Request</span></span>

<!-- { "blockType": "request", "name": "list-subsites" } -->

```http
GET /sites/{site-id}/sites
```

#### <a name="response"></a><span data-ttu-id="6aea1-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aea1-118">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Enumerate subsites"
} -->
