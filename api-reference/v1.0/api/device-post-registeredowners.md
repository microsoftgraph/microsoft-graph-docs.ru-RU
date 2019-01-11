---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 295c48c586a6ddf31b1ceef15b9f1137227ba3ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820526"
---
# <a name="create-registeredowner"></a><span data-ttu-id="87220-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="87220-103">Create registeredOwner</span></span>

<span data-ttu-id="87220-104">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="87220-104">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="87220-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87220-105">Permissions</span></span>
<span data-ttu-id="87220-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="87220-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87220-108">Permission type</span></span>      | <span data-ttu-id="87220-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87220-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87220-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87220-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87220-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="87220-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="87220-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87220-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87220-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87220-113">Not supported.</span></span>    |
|<span data-ttu-id="87220-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87220-114">Application</span></span> | <span data-ttu-id="87220-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87220-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87220-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87220-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="87220-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87220-117">Request headers</span></span>
| <span data-ttu-id="87220-118">Имя</span><span class="sxs-lookup"><span data-stu-id="87220-118">Name</span></span>       | <span data-ttu-id="87220-119">Тип</span><span class="sxs-lookup"><span data-stu-id="87220-119">Type</span></span> | <span data-ttu-id="87220-120">Описание</span><span class="sxs-lookup"><span data-stu-id="87220-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="87220-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87220-121">Authorization</span></span>  | <span data-ttu-id="87220-122">string</span><span class="sxs-lookup"><span data-stu-id="87220-122">string</span></span>  | <span data-ttu-id="87220-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87220-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87220-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87220-125">Request body</span></span>
<span data-ttu-id="87220-126">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87220-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="87220-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="87220-127">Response</span></span>

<span data-ttu-id="87220-128">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87220-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87220-129">Пример</span><span class="sxs-lookup"><span data-stu-id="87220-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87220-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="87220-130">Request</span></span>
<span data-ttu-id="87220-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87220-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="87220-132">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87220-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="87220-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="87220-133">Response</span></span>
<span data-ttu-id="87220-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87220-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
