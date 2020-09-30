---
title: Список удаленных элементов, принадлежащих пользователю
description: 'Получает список недавно удаленных элементов, принадлежащих указанному пользователю.  '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e3b001b7928cfcc008a1e1605d4effcd0cbd8e3b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48311940"
---
# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="dad77-103">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="dad77-103">List deleted items owned by a user</span></span>

<span data-ttu-id="dad77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad77-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dad77-105">Получает список недавно удаленных элементов, принадлежащих указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="dad77-105">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="dad77-106">В настоящее время функции списка удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md) и [группы](../resources/group.md) , принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="dad77-106">Currently, list deleted items functionality is supported only for [application](../resources/application.md) and [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="dad77-107">Это действие службы, которое означает, что она не поддерживает разбивку на страницы.</span><span class="sxs-lookup"><span data-stu-id="dad77-107">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="dad77-108">API возвращает до 1 000 удаленных объектов, принадлежащих пользователю, отсортированных по ИДЕНТИФИКАТОРу.</span><span class="sxs-lookup"><span data-stu-id="dad77-108">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="dad77-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dad77-109">Permissions</span></span>

<span data-ttu-id="dad77-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dad77-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dad77-112">Permission type</span></span> | <span data-ttu-id="dad77-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dad77-113">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="dad77-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dad77-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dad77-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad77-115">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="dad77-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dad77-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dad77-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dad77-117">Not supported.</span></span> |
| <span data-ttu-id="dad77-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dad77-118">Application</span></span> | <span data-ttu-id="dad77-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dad77-119">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dad77-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dad77-120">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="dad77-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dad77-121">Request headers</span></span>

| <span data-ttu-id="dad77-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dad77-122">Name</span></span>          | <span data-ttu-id="dad77-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dad77-123">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="dad77-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dad77-124">Authorization</span></span> | <span data-ttu-id="dad77-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dad77-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dad77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dad77-127">Request body</span></span>

<span data-ttu-id="dad77-128">В тексте запроса требуются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="dad77-128">The request body requires the following parameters:</span></span>

| <span data-ttu-id="dad77-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="dad77-129">Parameter</span></span>    | <span data-ttu-id="dad77-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dad77-130">Type</span></span> |<span data-ttu-id="dad77-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dad77-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dad77-132">userId</span><span class="sxs-lookup"><span data-stu-id="dad77-132">userId</span></span>|<span data-ttu-id="dad77-133">String</span><span class="sxs-lookup"><span data-stu-id="dad77-133">String</span></span>|<span data-ttu-id="dad77-134">Идентификатор владельца.</span><span class="sxs-lookup"><span data-stu-id="dad77-134">ID of the owner.</span></span>|
|<span data-ttu-id="dad77-135">type</span><span class="sxs-lookup"><span data-stu-id="dad77-135">type</span></span>|<span data-ttu-id="dad77-136">String</span><span class="sxs-lookup"><span data-stu-id="dad77-136">String</span></span>|<span data-ttu-id="dad77-137">Тип собственных объектов, которые требуется вернуть; в `group` настоящее время является единственным поддерживаемым значением.</span><span class="sxs-lookup"><span data-stu-id="dad77-137">Type of owned objects to return; `group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="dad77-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad77-138">Response</span></span>

<span data-ttu-id="dad77-139">Успешные запросы возвращают `200 OK` коды ответа; объект Response содержит свойства [Directory (удаленные элементы)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="dad77-139">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="dad77-140">Пример</span><span class="sxs-lookup"><span data-stu-id="dad77-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dad77-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="dad77-141">Request</span></span>

<span data-ttu-id="dad77-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dad77-142">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="dad77-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dad77-143">Response</span></span>

<span data-ttu-id="dad77-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dad77-144">Here is an example of the response.</span></span> <span data-ttu-id="dad77-145">Note: этот объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="dad77-145">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="dad77-146">Все поддерживаемые свойства возвращаются из фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="dad77-146">All supported properties are returned from actual calls.</span></span>

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