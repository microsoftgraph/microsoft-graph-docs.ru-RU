# <a name="group-renew"></a><span data-ttu-id="0ba7c-101">group: renew</span><span class="sxs-lookup"><span data-stu-id="0ba7c-101">group: renew</span></span>

<span data-ttu-id="0ba7c-102">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="0ba7c-102">Renews a group's expiration.</span></span> <span data-ttu-id="0ba7c-103">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="0ba7c-103">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ba7c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ba7c-104">Permissions</span></span>

<span data-ttu-id="0ba7c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ba7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="0ba7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ba7c-107">Permission type</span></span>      | <span data-ttu-id="0ba7c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ba7c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ba7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ba7c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0ba7c-110">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba7c-110">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0ba7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ba7c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ba7c-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0ba7c-112">Not supported</span></span> |
|<span data-ttu-id="0ba7c-113">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0ba7c-113">Application</span></span> | <span data-ttu-id="0ba7c-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba7c-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ba7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ba7c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a><span data-ttu-id="0ba7c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ba7c-116">Request headers</span></span>
| <span data-ttu-id="0ba7c-117">Имя</span><span class="sxs-lookup"><span data-stu-id="0ba7c-117">Name</span></span>       | <span data-ttu-id="0ba7c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0ba7c-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ba7c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ba7c-119">Authorization</span></span>  | <span data-ttu-id="0ba7c-120">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0ba7c-120">Bearer %token%</span></span> |


## <a name="request-body"></a><span data-ttu-id="0ba7c-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ba7c-121">Request body</span></span>

<span data-ttu-id="0ba7c-122">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ba7c-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ba7c-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ba7c-123">Response</span></span>

<span data-ttu-id="0ba7c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0ba7c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ba7c-126">Пример</span><span class="sxs-lookup"><span data-stu-id="0ba7c-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ba7c-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ba7c-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a><span data-ttu-id="0ba7c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ba7c-128">Response</span></span>
<span data-ttu-id="0ba7c-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ba7c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->