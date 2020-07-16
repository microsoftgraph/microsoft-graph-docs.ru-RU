---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4ed6fb6d236eb8c67400b75ee364a55c644ecfc
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146689"
---
# <a name="create-registereduser"></a><span data-ttu-id="643fa-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="643fa-103">Create registeredUser</span></span>

<span data-ttu-id="643fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="643fa-105">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="643fa-105">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="643fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="643fa-106">Permissions</span></span>
<span data-ttu-id="643fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="643fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="643fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="643fa-109">Permission type</span></span>      | <span data-ttu-id="643fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="643fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="643fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="643fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="643fa-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="643fa-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="643fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="643fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="643fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="643fa-114">Not supported.</span></span>    |
|<span data-ttu-id="643fa-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="643fa-115">Application</span></span> | <span data-ttu-id="643fa-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="643fa-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="643fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="643fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="643fa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="643fa-118">Request headers</span></span>
| <span data-ttu-id="643fa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="643fa-119">Name</span></span>       | <span data-ttu-id="643fa-120">Тип</span><span class="sxs-lookup"><span data-stu-id="643fa-120">Type</span></span> | <span data-ttu-id="643fa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="643fa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="643fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="643fa-122">Authorization</span></span>  | <span data-ttu-id="643fa-123">string</span><span class="sxs-lookup"><span data-stu-id="643fa-123">string</span></span>  | <span data-ttu-id="643fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="643fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="643fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="643fa-126">Request body</span></span>
<span data-ttu-id="643fa-127">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="643fa-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="643fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="643fa-128">Response</span></span>

<span data-ttu-id="643fa-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="643fa-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="643fa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="643fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="643fa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="643fa-131">Request</span></span>
<span data-ttu-id="643fa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="643fa-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="643fa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="643fa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/beta/devices/{id}/registeredUsers/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="643fa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="643fa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="643fa-135">C#</span><span class="sxs-lookup"><span data-stu-id="643fa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="643fa-136">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="643fa-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="643fa-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="643fa-137">Response</span></span>
<span data-ttu-id="643fa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="643fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
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
