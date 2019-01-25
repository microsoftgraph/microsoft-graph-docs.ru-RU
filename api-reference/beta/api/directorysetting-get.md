---
title: Получить параметры каталога
description: Извлечение свойств объекта параметр конкретного каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0ad7b0137e741ff6c6766980f121838ae00d8200
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525292"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="9e6ee-103">Получить параметры каталога</span><span class="sxs-lookup"><span data-stu-id="9e6ee-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6ee-104">Извлечение свойств объекта параметр конкретного каталога.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="9e6ee-105">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="9e6ee-106">Для *получения groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e6ee-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e6ee-107">Permissions</span></span>
<span data-ttu-id="9e6ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e6ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e6ee-110">Permission type</span></span>      | <span data-ttu-id="9e6ee-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e6ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e6ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e6ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9e6ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e6ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9e6ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e6ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e6ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-115">Not supported.</span></span>    |
|<span data-ttu-id="9e6ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e6ee-116">Application</span></span> | <span data-ttu-id="9e6ee-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6ee-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e6ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e6ee-118">HTTP request</span></span>
<span data-ttu-id="9e6ee-119"><!-- { "blockType": "ignored" } -->Получение определенных всей клиента или параметр групповой</span><span class="sxs-lookup"><span data-stu-id="9e6ee-119"><!-- { "blockType": "ignored" } --> Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e6ee-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9e6ee-120">Optional query parameters</span></span>
<span data-ttu-id="9e6ee-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e6ee-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e6ee-122">Request headers</span></span>
| <span data-ttu-id="9e6ee-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9e6ee-123">Name</span></span>      |<span data-ttu-id="9e6ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9e6ee-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e6ee-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9e6ee-125">Authorization</span></span>  | <span data-ttu-id="9e6ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6ee-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e6ee-128">Request body</span></span>
<span data-ttu-id="9e6ee-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e6ee-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e6ee-130">Response</span></span>

<span data-ttu-id="9e6ee-131">Успешно завершена, этот метод возвращает `200 OK` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e6ee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9e6ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e6ee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e6ee-133">Request</span></span>
<span data-ttu-id="9e6ee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e6ee-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="9e6ee-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e6ee-135">Response</span></span>
<span data-ttu-id="9e6ee-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9e6ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
