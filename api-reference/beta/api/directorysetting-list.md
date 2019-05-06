---
title: Параметры каталога списка
description: Получение списка объектов параметров каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1c41039c75a92c1b60e806680fd99d613823a624
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590131"
---
# <a name="list-directory-settings"></a><span data-ttu-id="d29bc-103">Параметры каталога списка</span><span class="sxs-lookup"><span data-stu-id="d29bc-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29bc-104">Получение списка объектов параметров каталога.</span><span class="sxs-lookup"><span data-stu-id="d29bc-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="d29bc-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="d29bc-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d29bc-106">Версия/v1.0 этого API была переименована в *List граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="d29bc-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d29bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d29bc-107">Permissions</span></span>
<span data-ttu-id="d29bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d29bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d29bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d29bc-110">Permission type</span></span>      | <span data-ttu-id="d29bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d29bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d29bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d29bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d29bc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d29bc-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d29bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d29bc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d29bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d29bc-115">Not supported.</span></span>    |
|<span data-ttu-id="d29bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d29bc-116">Application</span></span> | <span data-ttu-id="d29bc-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d29bc-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d29bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d29bc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d29bc-119">Перечисление параметров на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="d29bc-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d29bc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d29bc-120">Optional query parameters</span></span>
<span data-ttu-id="d29bc-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d29bc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d29bc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d29bc-122">Request headers</span></span>
| <span data-ttu-id="d29bc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d29bc-123">Name</span></span>      |<span data-ttu-id="d29bc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d29bc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d29bc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d29bc-125">Authorization</span></span>  | <span data-ttu-id="d29bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d29bc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d29bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d29bc-128">Request body</span></span>
<span data-ttu-id="d29bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d29bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d29bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d29bc-130">Response</span></span>

<span data-ttu-id="d29bc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d29bc-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d29bc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d29bc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d29bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d29bc-133">Request</span></span>
<span data-ttu-id="d29bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d29bc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="d29bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d29bc-135">Response</span></span>
<span data-ttu-id="d29bc-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d29bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d29bc-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="d29bc-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d29bc-140">Языках</span><span class="sxs-lookup"><span data-stu-id="d29bc-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_settings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d29bc-141">Язык</span><span class="sxs-lookup"><span data-stu-id="d29bc-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_settings-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
