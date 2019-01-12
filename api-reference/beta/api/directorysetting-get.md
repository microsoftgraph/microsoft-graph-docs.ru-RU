---
title: Получить параметры каталога
description: Извлечение свойств объекта параметр конкретного каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73953ccedeb7ecaeeba5cb68e6827956430ada82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950825"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="d8ce8-103">Получить параметры каталога</span><span class="sxs-lookup"><span data-stu-id="d8ce8-103">Get a directory setting</span></span>

> <span data-ttu-id="d8ce8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8ce8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8ce8-106">Извлечение свойств объекта параметр конкретного каталога.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="d8ce8-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d8ce8-108">Для *получения groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8ce8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8ce8-109">Permissions</span></span>
<span data-ttu-id="d8ce8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ce8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ce8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8ce8-112">Permission type</span></span>      | <span data-ttu-id="d8ce8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8ce8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8ce8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8ce8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d8ce8-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8ce8-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8ce8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8ce8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8ce8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-117">Not supported.</span></span>    |
|<span data-ttu-id="d8ce8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8ce8-118">Application</span></span> | <span data-ttu-id="d8ce8-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ce8-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8ce8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8ce8-120">HTTP request</span></span>
<span data-ttu-id="d8ce8-121"><!-- { "blockType": "ignored" } -->Получение определенных всей клиента или параметр групповой</span><span class="sxs-lookup"><span data-stu-id="d8ce8-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8ce8-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8ce8-122">Optional query parameters</span></span>
<span data-ttu-id="d8ce8-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8ce8-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8ce8-124">Request headers</span></span>
| <span data-ttu-id="d8ce8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d8ce8-125">Name</span></span>      |<span data-ttu-id="d8ce8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d8ce8-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8ce8-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8ce8-127">Authorization</span></span>  | <span data-ttu-id="d8ce8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8ce8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8ce8-130">Request body</span></span>
<span data-ttu-id="d8ce8-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8ce8-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8ce8-132">Response</span></span>

<span data-ttu-id="d8ce8-133">Успешно завершена, этот метод возвращает `200 OK` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8ce8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d8ce8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8ce8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8ce8-135">Request</span></span>
<span data-ttu-id="d8ce8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="d8ce8-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8ce8-137">Response</span></span>
<span data-ttu-id="d8ce8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8ce8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
