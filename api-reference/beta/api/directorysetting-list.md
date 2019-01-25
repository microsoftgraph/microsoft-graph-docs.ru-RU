---
title: Параметры каталога списка
description: Получение списка объектов параметр каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 708faad9dc90bf5f79f89d72b381391843371766
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515939"
---
# <a name="list-directory-settings"></a><span data-ttu-id="8b31c-103">Параметры каталога списка</span><span class="sxs-lookup"><span data-stu-id="8b31c-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b31c-104">Получение списка объектов параметр каталога.</span><span class="sxs-lookup"><span data-stu-id="8b31c-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="8b31c-105">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="8b31c-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="8b31c-106">Версия /v1.0 этот интерфейс API переименовано в *groupSettings списка*.</span><span class="sxs-lookup"><span data-stu-id="8b31c-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b31c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b31c-107">Permissions</span></span>
<span data-ttu-id="8b31c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b31c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b31c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b31c-110">Permission type</span></span>      | <span data-ttu-id="8b31c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b31c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b31c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b31c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b31c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b31c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b31c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b31c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b31c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b31c-115">Not supported.</span></span>    |
|<span data-ttu-id="8b31c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b31c-116">Application</span></span> | <span data-ttu-id="8b31c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b31c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b31c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b31c-118">HTTP request</span></span>
<span data-ttu-id="8b31c-119"><!-- { "blockType": "ignored" } -->Список всей клиента или параметры группы</span><span class="sxs-lookup"><span data-stu-id="8b31c-119"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b31c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b31c-120">Optional query parameters</span></span>
<span data-ttu-id="8b31c-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b31c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b31c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b31c-122">Request headers</span></span>
| <span data-ttu-id="8b31c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8b31c-123">Name</span></span>      |<span data-ttu-id="8b31c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8b31c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b31c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b31c-125">Authorization</span></span>  | <span data-ttu-id="8b31c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b31c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b31c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b31c-128">Request body</span></span>
<span data-ttu-id="8b31c-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b31c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b31c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b31c-130">Response</span></span>

<span data-ttu-id="8b31c-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [directorySetting](../resources/directorysetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b31c-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b31c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8b31c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b31c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b31c-133">Request</span></span>
<span data-ttu-id="8b31c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b31c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="8b31c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b31c-135">Response</span></span>
<span data-ttu-id="8b31c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8b31c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
