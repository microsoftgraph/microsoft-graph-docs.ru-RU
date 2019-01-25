---
title: Список directorySettingTemplates
description: Каталог установки шаблонов представляет набор шаблонов параметры каталога из каталога, который параметры могут быть созданы и используется внутри клиента.  Эта операция извлекает список доступных directorySettingTemplates объектов.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cd0112bd0d9f98f969832427d497d6e9ba2aa14
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530106"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="04fd0-104">Список directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="04fd0-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04fd0-105">Каталог установки шаблонов представляет набор шаблонов параметры каталога из каталога, который параметры могут быть созданы и используется внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="04fd0-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="04fd0-106">Эта операция извлекает список доступных directorySettingTemplates объектов.</span><span class="sxs-lookup"><span data-stu-id="04fd0-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="04fd0-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="04fd0-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="04fd0-108">Версия /v1.0 этот интерфейс API переименовано в *groupSettingTemplate списка*.</span><span class="sxs-lookup"><span data-stu-id="04fd0-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="04fd0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04fd0-109">Permissions</span></span>
<span data-ttu-id="04fd0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04fd0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04fd0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04fd0-112">Permission type</span></span>      | <span data-ttu-id="04fd0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04fd0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04fd0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04fd0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="04fd0-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04fd0-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04fd0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04fd0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04fd0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04fd0-117">Not supported.</span></span>    |
|<span data-ttu-id="04fd0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04fd0-118">Application</span></span> | <span data-ttu-id="04fd0-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04fd0-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04fd0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04fd0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="04fd0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04fd0-121">Optional query parameters</span></span>
<span data-ttu-id="04fd0-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="04fd0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04fd0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04fd0-123">Request headers</span></span>
| <span data-ttu-id="04fd0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="04fd0-124">Name</span></span>      |<span data-ttu-id="04fd0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="04fd0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04fd0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04fd0-126">Authorization</span></span>  | <span data-ttu-id="04fd0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04fd0-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04fd0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04fd0-129">Request body</span></span>
<span data-ttu-id="04fd0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04fd0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04fd0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="04fd0-131">Response</span></span>

<span data-ttu-id="04fd0-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [directorySettingTemplate](../resources/directorysettingtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="04fd0-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04fd0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="04fd0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04fd0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="04fd0-134">Request</span></span>
<span data-ttu-id="04fd0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04fd0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="04fd0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="04fd0-136">Response</span></span>
<span data-ttu-id="04fd0-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="04fd0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "description": "description-value",
      "values": [
        {
          "name": "name-value",
          "type": "type-value",
          "defaultValue": "defaultValue-value",
          "description": "description-value"
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
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
