---
title: 'directoryRole: Delta'
description: Получение только что созданных, обновленных или удаленных ролей каталогов без выполнения полного чтения всей коллекции ресурсов. Сведения об использовании запроса изменений см.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6da3e8c4cf92edbf79df1b082675c36d54e81292
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550604"
---
# <a name="directoryrole-delta"></a><span data-ttu-id="a1995-104">directoryRole: Delta</span><span class="sxs-lookup"><span data-stu-id="a1995-104">directoryRole: delta</span></span>

<span data-ttu-id="a1995-105">Получение только что созданных, обновленных или удаленных ролей каталогов без выполнения полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a1995-105">Get newly created, updated, or deleted directory roles without having to perform a full read of the entire resource collection.</span></span> <span data-ttu-id="a1995-106">Сведения об [использовании запроса изменений](/graph/delta-query-overview) см.</span><span class="sxs-lookup"><span data-stu-id="a1995-106">See [Using Delta Query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1995-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1995-107">Permissions</span></span>

<span data-ttu-id="a1995-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1995-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a1995-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1995-110">Permission type</span></span>      | <span data-ttu-id="a1995-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1995-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1995-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1995-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a1995-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a1995-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a1995-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1995-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1995-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1995-115">Not supported.</span></span>    |
|<span data-ttu-id="a1995-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1995-116">Application</span></span> | <span data-ttu-id="a1995-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1995-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1995-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1995-118">HTTP request</span></span>

<span data-ttu-id="a1995-119">Чтобы начать отслеживание изменений, создайте запрос, включающий функцию **Delta** в ресурсе [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="a1995-119">To begin tracking changes, you make a request including the **delta** function on the [directoryRole](../resources/directoryrole.md) resource.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/delta
```

## <a name="query-parameters"></a><span data-ttu-id="a1995-120">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="a1995-120">Query parameters</span></span>

<span data-ttu-id="a1995-121">Отслеживание изменений приводит к округлению одного или нескольких вызовов функции **Delta** .</span><span class="sxs-lookup"><span data-stu-id="a1995-121">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="a1995-122">Если вы используете любой параметр запроса (кроме `$deltatoken` и `$skiptoken`), необходимо указать его в исходном запросе **Delta** .</span><span class="sxs-lookup"><span data-stu-id="a1995-122">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="a1995-123">Microsoft Graph автоматически кодирует все заданные параметры в часть маркера или `nextLink` `deltaLink` URL-адрес, указанный в ответе.</span><span class="sxs-lookup"><span data-stu-id="a1995-123">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="a1995-124">Параметры запроса нужно указать только один раз в первом запросе.</span><span class="sxs-lookup"><span data-stu-id="a1995-124">You only need to specify any desired query parameters once upfront.</span></span> <span data-ttu-id="a1995-125">Копируйте и применяйте URL-адрес `nextLink` или `deltaLink` из предыдущего ответа в последующих запросах, так как в нем уже содержаться закодированные параметры.</span><span class="sxs-lookup"><span data-stu-id="a1995-125">In subsequent requests, copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="a1995-126">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="a1995-126">Query parameter</span></span>      | <span data-ttu-id="a1995-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a1995-127">Type</span></span>   |<span data-ttu-id="a1995-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a1995-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1995-129">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="a1995-129">$deltatoken</span></span> | <span data-ttu-id="a1995-130">string</span><span class="sxs-lookup"><span data-stu-id="a1995-130">string</span></span> | <span data-ttu-id="a1995-131">[Токен состояния](/graph/delta-query-overview) возвращается в `deltaLink` URL-адресе предыдущего вызова функции **Delta** для той же коллекции ресурсов, что указывает на завершение этого круга отслеживания изменений.</span><span class="sxs-lookup"><span data-stu-id="a1995-131">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same resource collection, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="a1995-132">Сохраните и примените весь `deltaLink` URL-адрес, включая этот маркер, в первом запросе следующего цикла отслеживания изменений для этой коллекции.</span><span class="sxs-lookup"><span data-stu-id="a1995-132">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that collection.</span></span>|
| <span data-ttu-id="a1995-133">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="a1995-133">$skiptoken</span></span> | <span data-ttu-id="a1995-134">string</span><span class="sxs-lookup"><span data-stu-id="a1995-134">string</span></span> | <span data-ttu-id="a1995-135">[Токен состояния](/graph/delta-query-overview) возвращается в `nextLink` URL-адресе предыдущего вызова функции **Delta** , указывая, что в коллекции ресурсов отслеживаются другие изменения.</span><span class="sxs-lookup"><span data-stu-id="a1995-135">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same resource collection.</span></span> |

### <a name="odata-query-parameters"></a><span data-ttu-id="a1995-136">Параметры запросов OData</span><span class="sxs-lookup"><span data-stu-id="a1995-136">OData query parameters</span></span>

<span data-ttu-id="a1995-137">Этот метод поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a1995-137">This method supports OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="a1995-p106">Вы можете использовать параметр запроса `$select` так же, как в любом другом запросе GET, чтобы задать только те свойства, которые необходимы для эффективной работы. Свойство _id_ возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="a1995-p106">You can use a `$select` query parameter as in any GET request to specify only the properties your need for best performance. The _id_ property is always returned.</span></span>

- <span data-ttu-id="a1995-140">Существует ограниченная поддержка `$filter`:</span><span class="sxs-lookup"><span data-stu-id="a1995-140">There is limited support for `$filter`:</span></span>

  - <span data-ttu-id="a1995-141">Единственное поддерживаемое `$filter` выражение предназначено для отслеживания изменений для определенных ресурсов по их идентификаторам: `$filter=id+eq+{value}` или `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span><span class="sxs-lookup"><span data-stu-id="a1995-141">The only supported `$filter` expression is for tracking changes for specific resources, by their id:  `$filter=id+eq+{value}` or `$filter=id+eq+{value1}+or+id+eq+{value2}`.</span></span> <span data-ttu-id="a1995-142">Количество идентификаторов, которые можно указать, ограничено максимальной длиной URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="a1995-142">The number of ids you can specify is limited by the maximum URL length.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1995-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1995-143">Request headers</span></span>

| <span data-ttu-id="a1995-144">Имя</span><span class="sxs-lookup"><span data-stu-id="a1995-144">Name</span></span>       | <span data-ttu-id="a1995-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a1995-145">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1995-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1995-146">Authorization</span></span>  | <span data-ttu-id="a1995-147">Bearer &lt;token&gt;</span><span class="sxs-lookup"><span data-stu-id="a1995-147">Bearer &lt;token&gt;</span></span>|
| <span data-ttu-id="a1995-148">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1995-148">Content-Type</span></span>  | <span data-ttu-id="a1995-149">application/json</span><span class="sxs-lookup"><span data-stu-id="a1995-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1995-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1995-150">Request body</span></span>

<span data-ttu-id="a1995-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1995-151">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a1995-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1995-152">Response</span></span>

<span data-ttu-id="a1995-153">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1995-153">If successful, this method returns `200 OK` response code and [directoryRole](../resources/directoryrole.md) collection object in the response body.</span></span> <span data-ttu-id="a1995-154">В ответ также включается `nextLink` URL-адрес `deltaLink` или URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="a1995-154">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="a1995-155">Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса получены не все страницы данных.</span><span class="sxs-lookup"><span data-stu-id="a1995-155">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="a1995-156">Приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в ответ не будет включен URL-адрес `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="a1995-156">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>

- <span data-ttu-id="a1995-157">Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса.</span><span class="sxs-lookup"><span data-stu-id="a1995-157">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="a1995-158">Сохраните `deltaLink` URL-адрес и примените его в следующем **Дельта** -вызове, чтобы узнать об изменениях в ресурсе в будущем.</span><span class="sxs-lookup"><span data-stu-id="a1995-158">Save `deltaLink` URL and apply it in the next **delta** call to learn about changes to the resource in the future.</span></span>

### <a name="example"></a><span data-ttu-id="a1995-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a1995-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a1995-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1995-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryRole_delta"
}-->

```http
GET https://graph.microsoft.com/v1.0/directoryRoles/delta
```

##### <a name="response"></a><span data-ttu-id="a1995-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1995-161">Response</span></span>

<span data-ttu-id="a1995-p111">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1995-p111">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryRoles",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/directoryRoles/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
      {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="a1995-164">См. также</span><span class="sxs-lookup"><span data-stu-id="a1995-164">See also</span></span>

- <span data-ttu-id="a1995-165">[Использование запроса изменений для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview) для получения дополнительных сведений</span><span class="sxs-lookup"><span data-stu-id="a1995-165">[Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview) for more details</span></span>
- <span data-ttu-id="a1995-166">[Примеры запросов](/graph/delta-query-users)</span><span class="sxs-lookup"><span data-stu-id="a1995-166">[Get incremental changes for users](/graph/delta-query-users) for an example requests.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
