---
title: Список удаленных элементов, которые принадлежат пользователю
description: 'Извлекает список недавно удаленных элементов, которые принадлежат указанному пользователю.  '
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 31a85be8a5c6b1dc09889ea77cf619060f702789
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436983"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="57f46-103">Список удаленных элементов, которые принадлежат пользователю</span><span class="sxs-lookup"><span data-stu-id="57f46-103">List deleted items owned by a user</span></span>

<span data-ttu-id="57f46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="57f46-105">Извлекает список недавно удаленных элементов, которые принадлежат указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="57f46-105">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="57f46-106">В настоящее время функции удаленных элементов списка поддерживаются только для [приложений](../resources/application.md) и групповых ресурсов, которые принадлежат пользователю. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="57f46-106">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="57f46-107">Это действие службы, которое означает, что оно не поддерживает pagination.</span><span class="sxs-lookup"><span data-stu-id="57f46-107">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="57f46-108">API возвращает до 1000 удаленных объектов, которые принадлежат пользователю, отсортировали по ID.</span><span class="sxs-lookup"><span data-stu-id="57f46-108">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="57f46-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57f46-109">Permissions</span></span>

<span data-ttu-id="57f46-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57f46-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57f46-112">Permission type</span></span> | <span data-ttu-id="57f46-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57f46-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="57f46-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57f46-114">Delegated (work or school account)</span></span> | <span data-ttu-id="57f46-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f46-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="57f46-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57f46-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="57f46-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57f46-117">Not supported.</span></span> |
| <span data-ttu-id="57f46-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="57f46-118">Application</span></span> | <span data-ttu-id="57f46-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57f46-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="57f46-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57f46-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="57f46-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57f46-121">Request headers</span></span>

| <span data-ttu-id="57f46-122">Имя</span><span class="sxs-lookup"><span data-stu-id="57f46-122">Name</span></span>          | <span data-ttu-id="57f46-123">Описание</span><span class="sxs-lookup"><span data-stu-id="57f46-123">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="57f46-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57f46-124">Authorization</span></span> | <span data-ttu-id="57f46-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57f46-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57f46-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57f46-127">Request body</span></span>

<span data-ttu-id="57f46-128">Орган запроса требует следующих параметров:</span><span class="sxs-lookup"><span data-stu-id="57f46-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="57f46-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="57f46-129">Parameter</span></span>    | <span data-ttu-id="57f46-130">Тип</span><span class="sxs-lookup"><span data-stu-id="57f46-130">Type</span></span> |<span data-ttu-id="57f46-131">Описание</span><span class="sxs-lookup"><span data-stu-id="57f46-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57f46-132">userId</span><span class="sxs-lookup"><span data-stu-id="57f46-132">userId</span></span>|<span data-ttu-id="57f46-133">String</span><span class="sxs-lookup"><span data-stu-id="57f46-133">String</span></span>|<span data-ttu-id="57f46-134">ID владельца.</span><span class="sxs-lookup"><span data-stu-id="57f46-134">ID of the owner.</span></span>|
|<span data-ttu-id="57f46-135">type</span><span class="sxs-lookup"><span data-stu-id="57f46-135">type</span></span>|<span data-ttu-id="57f46-136">String</span><span class="sxs-lookup"><span data-stu-id="57f46-136">String</span></span>|<span data-ttu-id="57f46-137">Тип объектов, которые необходимо возвращать; `group` в настоящее время является единственным поддерживаемым значением.</span><span class="sxs-lookup"><span data-stu-id="57f46-137">Type of owned objects to return; `group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="57f46-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="57f46-138">Response</span></span>

<span data-ttu-id="57f46-139">Успешные запросы возвращают коды ответов; объект ответа включает свойства `200 OK` [каталога (удаленных](../resources/directory.md) элементов).</span><span class="sxs-lookup"><span data-stu-id="57f46-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="57f46-140">Пример</span><span class="sxs-lookup"><span data-stu-id="57f46-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57f46-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="57f46-141">Request</span></span>

<span data-ttu-id="57f46-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57f46-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="57f46-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="57f46-143">Response</span></span>

<span data-ttu-id="57f46-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57f46-144">Here is an example of the response.</span></span> <span data-ttu-id="57f46-145">Примечание. Этот объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="57f46-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="57f46-146">Все поддерживаемые свойства возвращаются из фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="57f46-146">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
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
