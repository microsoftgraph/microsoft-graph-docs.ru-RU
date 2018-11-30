---
title: Список directorySettingTemplates
description: Каталог установки шаблонов представляет набор шаблонов параметры каталога из каталога, который параметры могут быть созданы и используется внутри клиента.  Эта операция извлекает список доступных directorySettingTemplates объектов.
ms.openlocfilehash: 964e2cfc9e06b6a996f63c92cae830e03c953cd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079376"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="441c9-104">Список directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="441c9-104">List directorySettingTemplates</span></span>

> <span data-ttu-id="441c9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="441c9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="441c9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441c9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="441c9-107">Каталог установки шаблонов представляет набор шаблонов параметры каталога из каталога, который параметры могут быть созданы и используется внутри клиента.</span><span class="sxs-lookup"><span data-stu-id="441c9-107">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="441c9-108">Эта операция извлекает список доступных directorySettingTemplates объектов.</span><span class="sxs-lookup"><span data-stu-id="441c9-108">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="441c9-109">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="441c9-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="441c9-110">Версия /v1.0 этот интерфейс API переименовано в *groupSettingTemplate списка*.</span><span class="sxs-lookup"><span data-stu-id="441c9-110">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="441c9-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="441c9-111">Permissions</span></span>
<span data-ttu-id="441c9-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="441c9-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="441c9-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="441c9-114">Permission type</span></span>      | <span data-ttu-id="441c9-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="441c9-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="441c9-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="441c9-116">Delegated (work or school account)</span></span> | <span data-ttu-id="441c9-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="441c9-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="441c9-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="441c9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="441c9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="441c9-119">Not supported.</span></span>    |
|<span data-ttu-id="441c9-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="441c9-120">Application</span></span> | <span data-ttu-id="441c9-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="441c9-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="441c9-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="441c9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="441c9-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="441c9-123">Optional query parameters</span></span>
<span data-ttu-id="441c9-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="441c9-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="441c9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="441c9-125">Request headers</span></span>
| <span data-ttu-id="441c9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="441c9-126">Name</span></span>      |<span data-ttu-id="441c9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="441c9-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="441c9-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="441c9-128">Authorization</span></span>  | <span data-ttu-id="441c9-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="441c9-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="441c9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="441c9-131">Request body</span></span>
<span data-ttu-id="441c9-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="441c9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="441c9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="441c9-133">Response</span></span>

<span data-ttu-id="441c9-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [directorySettingTemplate](../resources/directorysettingtemplate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="441c9-134">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="441c9-135">Пример</span><span class="sxs-lookup"><span data-stu-id="441c9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="441c9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="441c9-136">Request</span></span>
<span data-ttu-id="441c9-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="441c9-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="441c9-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="441c9-138">Response</span></span>
<span data-ttu-id="441c9-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="441c9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->