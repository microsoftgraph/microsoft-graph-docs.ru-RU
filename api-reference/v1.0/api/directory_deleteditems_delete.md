# <a name="permanently-delete-item"></a><span data-ttu-id="ee1ce-101">Удаление элемента без возможности восстановления</span><span class="sxs-lookup"><span data-stu-id="ee1ce-101">Permanently delete item</span></span>

<span data-ttu-id="ee1ce-102">Окончательное удаление элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ee1ce-102">Permanently deletes an item from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ee1ce-103">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ee1ce-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="ee1ce-104">Вы можете окончательно удалить элемент из папки "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="ee1ce-104">You can permanently delete an item from deleted items.</span></span> <span data-ttu-id="ee1ce-105">После окончательного удаления элемент **невозможно** восстановить.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-105">But, once an item is permanently deleted, it **cannot** be restored.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee1ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee1ce-106">Permissions</span></span>
<span data-ttu-id="ee1ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee1ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="ee1ce-109">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="ee1ce-109">For users:</span></span>

|<span data-ttu-id="ee1ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee1ce-110">Permission type</span></span>      | <span data-ttu-id="ee1ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee1ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ee1ce-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee1ce-113">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ee1ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee1ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-115">Not supported.</span></span> |
|<span data-ttu-id="ee1ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee1ce-116">Application</span></span> | <span data-ttu-id="ee1ce-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee1ce-117">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ee1ce-118">Для групп:</span><span class="sxs-lookup"><span data-stu-id="ee1ce-118">For groups:</span></span>

|<span data-ttu-id="ee1ce-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee1ce-119">Permission type</span></span>      | <span data-ttu-id="ee1ce-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee1ce-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ee1ce-122">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee1ce-122">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ee1ce-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee1ce-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee1ce-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-124">Not supported.</span></span>    |
|<span data-ttu-id="ee1ce-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee1ce-125">Application</span></span> | <span data-ttu-id="ee1ce-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee1ce-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee1ce-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee1ce-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/deleteditems/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ee1ce-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee1ce-128">Request headers</span></span>
| <span data-ttu-id="ee1ce-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ee1ce-129">Name</span></span>       | <span data-ttu-id="ee1ce-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ee1ce-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee1ce-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee1ce-131">Authorization</span></span>  | <span data-ttu-id="ee1ce-132">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-132">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ee1ce-133">Accept</span><span class="sxs-lookup"><span data-stu-id="ee1ce-133">Accept</span></span>  | <span data-ttu-id="ee1ce-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ee1ce-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee1ce-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee1ce-135">Request body</span></span>
<span data-ttu-id="ee1ce-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee1ce-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee1ce-137">Response</span></span>

<span data-ttu-id="ee1ce-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee1ce-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ee1ce-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee1ce-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee1ce-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_directory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="ee1ce-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee1ce-142">Response</span></span>
<span data-ttu-id="ee1ce-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee1ce-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->