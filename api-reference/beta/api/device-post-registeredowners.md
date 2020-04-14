---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbbc766b5b005a2d025e4d1fdd1dd14922587cc3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381776"
---
# <a name="create-registeredowner"></a><span data-ttu-id="9f950-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="9f950-103">Create registeredOwner</span></span>

<span data-ttu-id="9f950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f950-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f950-105">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="9f950-105">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f950-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f950-106">Permissions</span></span>
<span data-ttu-id="9f950-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9f950-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f950-109">Permission type</span></span>      | <span data-ttu-id="9f950-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f950-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f950-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f950-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f950-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f950-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f950-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f950-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f950-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f950-114">Not supported.</span></span>    |
|<span data-ttu-id="9f950-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9f950-115">Application</span></span> | <span data-ttu-id="9f950-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f950-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f950-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f950-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="9f950-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f950-118">Request headers</span></span>
| <span data-ttu-id="9f950-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f950-119">Name</span></span>       | <span data-ttu-id="9f950-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9f950-120">Type</span></span> | <span data-ttu-id="9f950-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9f950-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f950-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f950-122">Authorization</span></span>  | <span data-ttu-id="9f950-123">string</span><span class="sxs-lookup"><span data-stu-id="9f950-123">string</span></span>  | <span data-ttu-id="9f950-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f950-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f950-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f950-126">Request body</span></span>
<span data-ttu-id="9f950-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f950-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f950-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f950-128">Response</span></span>

<span data-ttu-id="9f950-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f950-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f950-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9f950-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f950-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f950-131">Request</span></span>
<span data-ttu-id="9f950-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f950-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f950-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f950-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredOwners/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="9f950-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f950-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9f950-135">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f950-135">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9f950-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f950-136">Response</span></span>
<span data-ttu-id="9f950-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f950-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
