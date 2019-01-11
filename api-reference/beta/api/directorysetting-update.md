---
title: Обновите параметр каталога
description: Обновление свойства объекта параметр конкретного каталога.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: f1c4c4c408f287fe6bfcf84eed3599aa85e3afbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843353"
---
# <a name="update-a-directory-setting"></a><span data-ttu-id="132ae-103">Обновите параметр каталога</span><span class="sxs-lookup"><span data-stu-id="132ae-103">Update a directory setting</span></span>

> <span data-ttu-id="132ae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="132ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="132ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="132ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="132ae-106">Обновление свойства объекта параметр конкретного каталога.</span><span class="sxs-lookup"><span data-stu-id="132ae-106">Update the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="132ae-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="132ae-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="132ae-108">Для *обновления groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="132ae-108">The /v1.0 version of this API has been renamed to *Update groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="132ae-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="132ae-109">Permissions</span></span>
<span data-ttu-id="132ae-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="132ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="132ae-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="132ae-112">Permission type</span></span>      | <span data-ttu-id="132ae-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="132ae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="132ae-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="132ae-114">Delegated (work or school account)</span></span> | <span data-ttu-id="132ae-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="132ae-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="132ae-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="132ae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="132ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="132ae-117">Not supported.</span></span>    |
|<span data-ttu-id="132ae-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="132ae-118">Application</span></span> | <span data-ttu-id="132ae-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="132ae-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="132ae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="132ae-120">HTTP request</span></span>
<span data-ttu-id="132ae-121"><!-- { "blockType": "ignored" } -->Обновление клиента всей или группу параметров.</span><span class="sxs-lookup"><span data-stu-id="132ae-121"><!-- { "blockType": "ignored" } --> Update a tenant-wide or group specific setting.</span></span>
```http
PATCH /settings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="132ae-122">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="132ae-122">Optional request headers</span></span>
| <span data-ttu-id="132ae-123">Имя</span><span class="sxs-lookup"><span data-stu-id="132ae-123">Name</span></span>       | <span data-ttu-id="132ae-124">Описание</span><span class="sxs-lookup"><span data-stu-id="132ae-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="132ae-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="132ae-125">Authorization</span></span>  | <span data-ttu-id="132ae-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="132ae-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="132ae-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="132ae-128">Request body</span></span>
<span data-ttu-id="132ae-129">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="132ae-129">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="132ae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="132ae-130">Property</span></span>     | <span data-ttu-id="132ae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="132ae-131">Type</span></span>   |<span data-ttu-id="132ae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="132ae-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="132ae-133">values</span><span class="sxs-lookup"><span data-stu-id="132ae-133">values</span></span> | <span data-ttu-id="132ae-134">settingValue</span><span class="sxs-lookup"><span data-stu-id="132ae-134">settingValue</span></span> | <span data-ttu-id="132ae-p105">Обновленный набор значений.  ПРИМЕЧАНИЕ. Необходимо предоставить весь набор коллекции. Вы не можете обновить отдельный набор значений.</span><span class="sxs-lookup"><span data-stu-id="132ae-p105">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="132ae-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="132ae-138">Response</span></span>

<span data-ttu-id="132ae-139">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="132ae-139">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="132ae-140">Пример</span><span class="sxs-lookup"><span data-stu-id="132ae-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="132ae-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="132ae-141">Request</span></span>
<span data-ttu-id="132ae-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="132ae-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_directorysetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/settings/{id}
Content-type: application/json
Content-length: 178

{
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="132ae-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="132ae-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorysetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update directorysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
