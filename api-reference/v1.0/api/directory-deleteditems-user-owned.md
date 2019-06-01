---
title: Разрешения
description: 'Получает список недавно удаленных элементов, принадлежащих указанному пользователю.  '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 75d943a37899b6f1d84971305cd473a398b049bb
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656659"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="4e68b-103">**Список удаленных элементов, принадлежащих пользователю**</span><span class="sxs-lookup"><span data-stu-id="4e68b-103">**List deleted items owned by a user**</span></span>

<span data-ttu-id="4e68b-104">Получает список недавно удаленных элементов, принадлежащих указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="4e68b-104">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="4e68b-105">В настоящее время функции списка удаленных элементов поддерживаются только для ресурсов [группы](../resources/group.md) , принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="4e68b-105">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="4e68b-106">Это действие службы, которое означает, что она не поддерживает разбивку на страницы.</span><span class="sxs-lookup"><span data-stu-id="4e68b-106">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="4e68b-107">API возвращает до 1 000 удаленных объектов, принадлежащих пользователю, отсортированных по ИДЕНТИФИКАТОРу.</span><span class="sxs-lookup"><span data-stu-id="4e68b-107">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e68b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e68b-108">Permissions</span></span>

<span data-ttu-id="4e68b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="4e68b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="4e68b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e68b-111">Permission type</span></span> | <span data-ttu-id="4e68b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e68b-112">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="4e68b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e68b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4e68b-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e68b-114">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4e68b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e68b-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4e68b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e68b-116">Not supported.</span></span> |
| <span data-ttu-id="4e68b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e68b-117">Application</span></span> | <span data-ttu-id="4e68b-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e68b-118">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4e68b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e68b-119">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="4e68b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e68b-120">Request headers</span></span>

| <span data-ttu-id="4e68b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4e68b-121">Name</span></span>          | <span data-ttu-id="4e68b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4e68b-122">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="4e68b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e68b-123">Authorization</span></span> | <span data-ttu-id="4e68b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e68b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e68b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e68b-126">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="4e68b-127">В тексте запроса требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="4e68b-127">The request body requires the following parameters:</span></span>

| <span data-ttu-id="4e68b-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e68b-128">Parameter</span></span>    | <span data-ttu-id="4e68b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4e68b-129">Type</span></span> |<span data-ttu-id="4e68b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4e68b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e68b-131">userId</span><span class="sxs-lookup"><span data-stu-id="4e68b-131">userId</span></span>|<span data-ttu-id="4e68b-132">String</span><span class="sxs-lookup"><span data-stu-id="4e68b-132">String</span></span>|<span data-ttu-id="4e68b-133">Идентификатор владельца.</span><span class="sxs-lookup"><span data-stu-id="4e68b-133">ID of the owner.</span></span>|
|<span data-ttu-id="4e68b-134">type</span><span class="sxs-lookup"><span data-stu-id="4e68b-134">type</span></span>|<span data-ttu-id="4e68b-135">String</span><span class="sxs-lookup"><span data-stu-id="4e68b-135">String</span></span>|<span data-ttu-id="4e68b-136">Тип собственных объектов, которые требуется вернуть; `Group` в настоящее время является единственным поддерживаемым значением.</span><span class="sxs-lookup"><span data-stu-id="4e68b-136">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="4e68b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e68b-137">Response</span></span>

<span data-ttu-id="4e68b-138">Успешные запросы `200 OK` возвращают коды ответа; объект Response содержит свойства [Directory (удаленные элементы)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="4e68b-138">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="4e68b-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4e68b-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4e68b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e68b-140">Request</span></span>

<span data-ttu-id="4e68b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e68b-141">Here is an example of the request.</span></span>

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

###### <a name="response"></a><span data-ttu-id="4e68b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e68b-142">Response</span></span>

<span data-ttu-id="4e68b-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e68b-143">Here is an example of the response.</span></span> <span data-ttu-id="4e68b-144">Note: этот объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4e68b-144">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="4e68b-145">Все поддерживаемые свойства возвращаются из фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="4e68b-145">All supported properties are returned from actual calls.</span></span>

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


