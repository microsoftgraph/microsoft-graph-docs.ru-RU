---
title: Создание объекта registeredUser
description: Добавление зарегистрированного пользователя устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4ebc3bd068300eeda1d56ae974f8c9c13a74d61
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916560"
---
# <a name="create-registereduser"></a><span data-ttu-id="db668-103">Создание объекта registeredUser</span><span class="sxs-lookup"><span data-stu-id="db668-103">Create registeredUser</span></span>

> <span data-ttu-id="db668-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db668-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db668-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db668-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db668-106">Добавление зарегистрированного пользователя устройства.</span><span class="sxs-lookup"><span data-stu-id="db668-106">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="db668-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db668-107">Permissions</span></span>
<span data-ttu-id="db668-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db668-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="db668-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db668-110">Permission type</span></span>      | <span data-ttu-id="db668-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db668-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db668-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db668-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db668-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db668-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db668-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db668-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db668-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db668-115">Not supported.</span></span>    |
|<span data-ttu-id="db668-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db668-116">Application</span></span> | <span data-ttu-id="db668-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db668-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db668-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db668-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers/$ref

```
## <a name="request-headers"></a><span data-ttu-id="db668-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db668-119">Request headers</span></span>
| <span data-ttu-id="db668-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db668-120">Name</span></span>       | <span data-ttu-id="db668-121">Тип</span><span class="sxs-lookup"><span data-stu-id="db668-121">Type</span></span> | <span data-ttu-id="db668-122">Описание</span><span class="sxs-lookup"><span data-stu-id="db668-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db668-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db668-123">Authorization</span></span>  | <span data-ttu-id="db668-124">строка</span><span class="sxs-lookup"><span data-stu-id="db668-124">string</span></span>  | <span data-ttu-id="db668-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db668-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db668-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db668-127">Request body</span></span>
<span data-ttu-id="db668-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db668-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db668-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="db668-129">Response</span></span>

<span data-ttu-id="db668-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db668-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db668-131">Пример</span><span class="sxs-lookup"><span data-stu-id="db668-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db668-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="db668-132">Request</span></span>
<span data-ttu-id="db668-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db668-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="db668-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db668-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="db668-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="db668-135">Response</span></span>
<span data-ttu-id="db668-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="db668-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
