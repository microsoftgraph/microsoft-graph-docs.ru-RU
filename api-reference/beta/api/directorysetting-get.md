---
title: Получить параметры каталога
description: Извлечение свойств объекта параметр конкретного каталога.
author: lleonard-msft
ms.openlocfilehash: 7dfd6d7f7623aef082a43c0b67c1867edb691f31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361476"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="d6a75-103">Получить параметры каталога</span><span class="sxs-lookup"><span data-stu-id="d6a75-103">Get a directory setting</span></span>

> <span data-ttu-id="d6a75-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6a75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6a75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6a75-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6a75-106">Извлечение свойств объекта параметр конкретного каталога.</span><span class="sxs-lookup"><span data-stu-id="d6a75-106">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="d6a75-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="d6a75-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d6a75-108">Для *получения groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="d6a75-108">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6a75-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6a75-109">Permissions</span></span>
<span data-ttu-id="d6a75-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6a75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6a75-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6a75-112">Permission type</span></span>      | <span data-ttu-id="d6a75-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6a75-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6a75-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6a75-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d6a75-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d6a75-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6a75-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6a75-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6a75-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6a75-117">Not supported.</span></span>    |
|<span data-ttu-id="d6a75-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6a75-118">Application</span></span> | <span data-ttu-id="d6a75-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6a75-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6a75-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6a75-120">HTTP request</span></span>
<span data-ttu-id="d6a75-121"><!-- { "blockType": "ignored" } -->Получение определенных всей клиента или параметр групповой</span><span class="sxs-lookup"><span data-stu-id="d6a75-121"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6a75-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d6a75-122">Optional query parameters</span></span>
<span data-ttu-id="d6a75-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d6a75-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6a75-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6a75-124">Request headers</span></span>
| <span data-ttu-id="d6a75-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d6a75-125">Name</span></span>      |<span data-ttu-id="d6a75-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d6a75-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d6a75-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6a75-127">Authorization</span></span>  | <span data-ttu-id="d6a75-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6a75-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6a75-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6a75-130">Request body</span></span>
<span data-ttu-id="d6a75-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6a75-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6a75-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6a75-132">Response</span></span>

<span data-ttu-id="d6a75-133">Успешно завершена, этот метод возвращает `200 OK` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d6a75-133">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6a75-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d6a75-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6a75-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6a75-135">Request</span></span>
<span data-ttu-id="d6a75-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6a75-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="d6a75-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6a75-137">Response</span></span>
<span data-ttu-id="d6a75-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d6a75-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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