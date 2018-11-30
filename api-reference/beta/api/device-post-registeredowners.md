---
title: Создание объекта registeredOwner
description: Добавление пользователя в качестве зарегистрированного владельца устройства.
ms.openlocfilehash: 767b28d8af9c26c336e36698024d89dac7f97786
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075260"
---
# <a name="create-registeredowner"></a><span data-ttu-id="4103e-103">Создание объекта registeredOwner</span><span class="sxs-lookup"><span data-stu-id="4103e-103">Create registeredOwner</span></span>

> <span data-ttu-id="4103e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4103e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4103e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4103e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4103e-106">Добавление пользователя в качестве зарегистрированного владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="4103e-106">Add a user as a registered owner of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="4103e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4103e-107">Permissions</span></span>
<span data-ttu-id="4103e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4103e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4103e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4103e-110">Permission type</span></span>      | <span data-ttu-id="4103e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4103e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4103e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4103e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4103e-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4103e-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4103e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4103e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4103e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4103e-115">Not supported.</span></span>    |
|<span data-ttu-id="4103e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4103e-116">Application</span></span> | <span data-ttu-id="4103e-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4103e-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4103e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4103e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="4103e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4103e-119">Request headers</span></span>
| <span data-ttu-id="4103e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4103e-120">Name</span></span>       | <span data-ttu-id="4103e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4103e-121">Type</span></span> | <span data-ttu-id="4103e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4103e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4103e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4103e-123">Authorization</span></span>  | <span data-ttu-id="4103e-124">string</span><span class="sxs-lookup"><span data-stu-id="4103e-124">string</span></span>  | <span data-ttu-id="4103e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4103e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4103e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4103e-127">Request body</span></span>
<span data-ttu-id="4103e-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4103e-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4103e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4103e-129">Response</span></span>

<span data-ttu-id="4103e-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4103e-130">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4103e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4103e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4103e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4103e-132">Request</span></span>
<span data-ttu-id="4103e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4103e-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="4103e-134">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4103e-134">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4103e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4103e-135">Response</span></span>
<span data-ttu-id="4103e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4103e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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