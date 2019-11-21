---
title: 'Device: Чеккмемберобжектс'
description: Проверка членства в списке групп или ролей каталогов для указанного объекта Device.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 536781e0a91a88c600d7478f8d93c10db7e66f42
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757327"
---
# <a name="device-checkmemberobjects"></a><span data-ttu-id="4d750-103">Device: Чеккмемберобжектс</span><span class="sxs-lookup"><span data-stu-id="4d750-103">device: checkMemberObjects</span></span>

<span data-ttu-id="4d750-104">Проверка членства в списке групп или ролей каталогов для указанного объекта Device.</span><span class="sxs-lookup"><span data-stu-id="4d750-104">Check for membership in a list of groups or directory roles for the specified device object.</span></span> <span data-ttu-id="4d750-105">Этот метод является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="4d750-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d750-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d750-106">Permissions</span></span>

<span data-ttu-id="4d750-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d750-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d750-109">Permission type</span></span>                        | <span data-ttu-id="4d750-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d750-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d750-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d750-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d750-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d750-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4d750-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d750-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d750-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d750-114">Not supported.</span></span> |
| <span data-ttu-id="4d750-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d750-115">Application</span></span>                            | <span data-ttu-id="4d750-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d750-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d750-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d750-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="4d750-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d750-118">Request headers</span></span>

| <span data-ttu-id="4d750-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4d750-119">Name</span></span>          | <span data-ttu-id="4d750-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4d750-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d750-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d750-121">Authorization</span></span> | <span data-ttu-id="4d750-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d750-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d750-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d750-124">Content-Type</span></span>  | <span data-ttu-id="4d750-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d750-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d750-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d750-127">Request body</span></span>

<span data-ttu-id="4d750-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4d750-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d750-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d750-129">Parameter</span></span>    | <span data-ttu-id="4d750-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4d750-130">Type</span></span>        | <span data-ttu-id="4d750-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4d750-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4d750-132">ids</span><span class="sxs-lookup"><span data-stu-id="4d750-132">ids</span></span> | <span data-ttu-id="4d750-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4d750-133">String collection</span></span> | <span data-ttu-id="4d750-134">Коллекция, содержащая идентификаторы объектов групп, ролей каталогов или идентификаторов Ролетемплате для ролей каталогов, в которых проверяется членство.</span><span class="sxs-lookup"><span data-stu-id="4d750-134">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="4d750-135">Можно указать до 20 объектов.</span><span class="sxs-lookup"><span data-stu-id="4d750-135">You can specify up to 20 objects.</span></span> |

## <a name="response"></a><span data-ttu-id="4d750-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d750-136">Response</span></span>

<span data-ttu-id="4d750-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d750-137">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d750-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d750-138">Examples</span></span>

<span data-ttu-id="4d750-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4d750-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4d750-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d750-140">Request</span></span>

<span data-ttu-id="4d750-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d750-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d750-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d750-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "device_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/devices/{id}/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4d750-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d750-143">Response</span></span>

<span data-ttu-id="4d750-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d750-144">The following is an example of the response.</span></span> 

> <span data-ttu-id="4d750-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d750-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
