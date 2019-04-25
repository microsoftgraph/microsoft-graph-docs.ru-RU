---
title: Удаление объекта calendarGroup
description: Удаление группы календарей, отличной от стандартной.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f1dded8885f99646d48ddf309ff12e64d61988e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572698"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="a03c5-103">Удаление объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a03c5-103">Delete calendarGroup</span></span>

<span data-ttu-id="a03c5-104">Удаление группы календарей, отличной от стандартной.</span><span class="sxs-lookup"><span data-stu-id="a03c5-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a03c5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a03c5-105">Permissions</span></span>

<span data-ttu-id="a03c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a03c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a03c5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a03c5-108">Permission type</span></span>                        | <span data-ttu-id="a03c5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a03c5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a03c5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a03c5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a03c5-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c5-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a03c5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a03c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a03c5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c5-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="a03c5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a03c5-114">Application</span></span>                            | <span data-ttu-id="a03c5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a03c5-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a03c5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a03c5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a03c5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a03c5-117">Request headers</span></span>

| <span data-ttu-id="a03c5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a03c5-118">Name</span></span>          | <span data-ttu-id="a03c5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a03c5-119">Type</span></span>   | <span data-ttu-id="a03c5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a03c5-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a03c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a03c5-121">Authorization</span></span> | <span data-ttu-id="a03c5-122">string</span><span class="sxs-lookup"><span data-stu-id="a03c5-122">string</span></span> | <span data-ttu-id="a03c5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a03c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a03c5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a03c5-125">Request body</span></span>

<span data-ttu-id="a03c5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a03c5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a03c5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a03c5-127">Response</span></span>

<span data-ttu-id="a03c5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a03c5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a03c5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a03c5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a03c5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a03c5-131">Request</span></span>

<span data-ttu-id="a03c5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a03c5-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="a03c5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a03c5-133">Response</span></span>

<span data-ttu-id="a03c5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a03c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
