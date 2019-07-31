---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 040974c2bc7ed29217e7a78cab5ff257fbb35752
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951325"
---
# <a name="create-registereduser"></a><span data-ttu-id="8db61-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="8db61-103">Create registeredUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8db61-104">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="8db61-104">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="8db61-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8db61-105">Permissions</span></span>
<span data-ttu-id="8db61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8db61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8db61-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8db61-108">Permission type</span></span>      | <span data-ttu-id="8db61-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8db61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8db61-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8db61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8db61-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8db61-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8db61-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8db61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8db61-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8db61-113">Not supported.</span></span>    |
|<span data-ttu-id="8db61-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8db61-114">Application</span></span> | <span data-ttu-id="8db61-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8db61-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8db61-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8db61-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="8db61-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8db61-117">Request headers</span></span>
| <span data-ttu-id="8db61-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8db61-118">Name</span></span>       | <span data-ttu-id="8db61-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8db61-119">Type</span></span> | <span data-ttu-id="8db61-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8db61-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8db61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8db61-121">Authorization</span></span>  | <span data-ttu-id="8db61-122">string</span><span class="sxs-lookup"><span data-stu-id="8db61-122">string</span></span>  | <span data-ttu-id="8db61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8db61-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8db61-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8db61-125">Request body</span></span>
<span data-ttu-id="8db61-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8db61-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8db61-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8db61-127">Response</span></span>

<span data-ttu-id="8db61-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8db61-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8db61-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8db61-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8db61-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8db61-130">Request</span></span>
<span data-ttu-id="8db61-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8db61-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8db61-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8db61-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8db61-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="8db61-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8db61-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8db61-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8db61-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8db61-135">Response</span></span>
<span data-ttu-id="8db61-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8db61-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
