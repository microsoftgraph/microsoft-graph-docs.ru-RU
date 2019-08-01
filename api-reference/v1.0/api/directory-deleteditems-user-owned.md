---
title: Разрешения
description: 'Получает список недавно удаленных элементов, принадлежащих указанному пользователю.  '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0a863964f553bedeb4e47c81afefc3aa4f7d39b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016939"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="00e5c-103">**Список удаленных элементов, принадлежащих пользователю**</span><span class="sxs-lookup"><span data-stu-id="00e5c-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="00e5c-104">Получает список недавно удаленных элементов, принадлежащих указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="00e5c-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="00e5c-105">В настоящее время функции списка удаленных элементов поддерживаются только для ресурсов [группы](../resources/group.md) , принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="00e5c-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="00e5c-106">Это действие службы, которое означает, что она не поддерживает разбивку на страницы.</span><span class="sxs-lookup"><span data-stu-id="00e5c-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="00e5c-107">API возвращает до 1 000 удаленных объектов, принадлежащих пользователю, отсортированных по ИДЕНТИФИКАТОРу.</span><span class="sxs-lookup"><span data-stu-id="00e5c-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e5c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00e5c-108">Permissions</span></span>

<span data-ttu-id="00e5c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="00e5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="00e5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00e5c-111">Permission type</span></span> | <span data-ttu-id="00e5c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00e5c-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="00e5c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00e5c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="00e5c-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e5c-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="00e5c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00e5c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00e5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00e5c-116">Not supported.</span></span> |
| <span data-ttu-id="00e5c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00e5c-117">Application</span></span> | <span data-ttu-id="00e5c-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00e5c-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="00e5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00e5c-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="00e5c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00e5c-120">Request headers</span></span>

| <span data-ttu-id="00e5c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="00e5c-121">Name</span></span>          | <span data-ttu-id="00e5c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="00e5c-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="00e5c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00e5c-123">Authorization</span></span> | <span data-ttu-id="00e5c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00e5c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00e5c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00e5c-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="00e5c-127">В тексте запроса требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="00e5c-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="00e5c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="00e5c-128">Parameter</span></span>    | <span data-ttu-id="00e5c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="00e5c-129">Type</span></span> |<span data-ttu-id="00e5c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="00e5c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00e5c-131">userId</span><span class="sxs-lookup"><span data-stu-id="00e5c-131">userId</span></span>|<span data-ttu-id="00e5c-132">String</span><span class="sxs-lookup"><span data-stu-id="00e5c-132">String</span></span>|<span data-ttu-id="00e5c-133">Идентификатор владельца.</span><span class="sxs-lookup"><span data-stu-id="00e5c-133">ID of the owner.</span></span>|
|<span data-ttu-id="00e5c-134">type</span><span class="sxs-lookup"><span data-stu-id="00e5c-134">type</span></span>|<span data-ttu-id="00e5c-135">String</span><span class="sxs-lookup"><span data-stu-id="00e5c-135">String</span></span>|<span data-ttu-id="00e5c-136">Тип собственных объектов, которые требуется вернуть; `Group` в настоящее время является единственным поддерживаемым значением.</span><span class="sxs-lookup"><span data-stu-id="00e5c-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="00e5c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="00e5c-137">Response</span></span>

<span data-ttu-id="00e5c-138">Успешные запросы `200 OK` возвращают коды ответа; объект Response содержит свойства [Directory (удаленные элементы)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="00e5c-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="00e5c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="00e5c-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="00e5c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="00e5c-140">Request</span></span>

<span data-ttu-id="00e5c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00e5c-141">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="00e5c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="00e5c-142">Response</span></span>

<span data-ttu-id="00e5c-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00e5c-143">Here is an example of the response.</span></span> <span data-ttu-id="00e5c-144">Note: этот объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="00e5c-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="00e5c-145">Все поддерживаемые свойства возвращаются из фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="00e5c-145">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
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


