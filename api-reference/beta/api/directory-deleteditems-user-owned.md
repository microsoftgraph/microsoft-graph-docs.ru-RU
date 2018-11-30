---
title: Permissions
description: 'Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.  '
ms.openlocfilehash: 6d455fc7646c7e9c2b3fb62f48e098a5daeacff2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079794"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="7bae7-103">**Список удаленных элементов, принадлежащие пользователю**</span><span class="sxs-lookup"><span data-stu-id="7bae7-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="7bae7-104">Извлекает список недавно удаленных элементов, принадлежащие указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="7bae7-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="7bae7-105">На данный момент удаленных элементов со списками поддерживается только для [группы](../resources/group.md) ресурсов владеет пользователь.</span><span class="sxs-lookup"><span data-stu-id="7bae7-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="7bae7-106">Это действие службы, которое означает, что он не поддерживает разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="7bae7-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="7bae7-107">API возвращает до 1 000 удаленных объектов, принадлежащие пользователю, отсортированные по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="7bae7-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>  <span data-ttu-id="7bae7-108">1000 или больше удаленных владеет пользователь объектов API возвращает значение nothing.</span><span class="sxs-lookup"><span data-stu-id="7bae7-108">Should the user own 1,000 or more deleted objects, the API returns nothing.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bae7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bae7-109">Permissions</span></span>

<span data-ttu-id="7bae7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7bae7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="7bae7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bae7-112">Permission type</span></span> | <span data-ttu-id="7bae7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bae7-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="7bae7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bae7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7bae7-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bae7-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7bae7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bae7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7bae7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bae7-117">Not supported.</span></span> |
| <span data-ttu-id="7bae7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bae7-118">Application</span></span> | <span data-ttu-id="7bae7-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bae7-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7bae7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bae7-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="7bae7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bae7-121">Request headers</span></span>

| <span data-ttu-id="7bae7-122">**Имя**</span><span class="sxs-lookup"><span data-stu-id="7bae7-122">**Name**</span></span>      | <span data-ttu-id="7bae7-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7bae7-123">**Description**</span></span>           |
| ------------- | ------------------------- |
| <span data-ttu-id="7bae7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bae7-124">Authorization</span></span> | <span data-ttu-id="7bae7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bae7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bae7-127">Request body</span></span>

```json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

<span data-ttu-id="7bae7-128">Текст запроса необходимо задать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="7bae7-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="7bae7-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7bae7-129">Parameter</span></span>    | <span data-ttu-id="7bae7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7bae7-130">Type</span></span> |<span data-ttu-id="7bae7-131">Description</span><span class="sxs-lookup"><span data-stu-id="7bae7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bae7-132">userId</span><span class="sxs-lookup"><span data-stu-id="7bae7-132">userId</span></span>|<span data-ttu-id="7bae7-133">String</span><span class="sxs-lookup"><span data-stu-id="7bae7-133">String</span></span>|<span data-ttu-id="7bae7-134">Идентификатор владельца.</span><span class="sxs-lookup"><span data-stu-id="7bae7-134">ID of the owner.</span></span>|
|<span data-ttu-id="7bae7-135">type</span><span class="sxs-lookup"><span data-stu-id="7bae7-135">type</span></span>|<span data-ttu-id="7bae7-136">String</span><span class="sxs-lookup"><span data-stu-id="7bae7-136">String</span></span>|<span data-ttu-id="7bae7-137">Тип собственные объекты для возвращения; `Group` в данный момент поддерживается только значение.</span><span class="sxs-lookup"><span data-stu-id="7bae7-137">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|

## <a name="response"></a><span data-ttu-id="7bae7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bae7-138">Response</span></span>

<span data-ttu-id="7bae7-139">Успешные запросы `200 OK` коды ответа; объект ответа включает в себя свойств [каталога (удаленных элементов)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="7bae7-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="7bae7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7bae7-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7bae7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bae7-141">Request</span></span>

<span data-ttu-id="7bae7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bae7-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"Group"
}
```

###### <a name="response"></a><span data-ttu-id="7bae7-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bae7-143">Response</span></span>

<span data-ttu-id="7bae7-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bae7-144">Here is an example of the response.</span></span> <span data-ttu-id="7bae7-145">Примечание: Этот объект ответа может усекаться для краткости.</span><span class="sxs-lookup"><span data-stu-id="7bae7-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="7bae7-146">Все поддерживаемые свойства возвращаются фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="7bae7-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:34:56Z",
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


