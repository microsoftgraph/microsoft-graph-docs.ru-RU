---
title: Параметры каталога списка
description: Получение списка объектов параметр каталога.
ms.openlocfilehash: 844d2102b9bfd98e2ba0a585a7eb04c8e46b6a52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075955"
---
# <a name="list-directory-settings"></a><span data-ttu-id="1f627-103">Параметры каталога списка</span><span class="sxs-lookup"><span data-stu-id="1f627-103">List directory settings</span></span>

> <span data-ttu-id="1f627-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f627-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f627-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f627-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f627-106">Получение списка объектов параметр каталога.</span><span class="sxs-lookup"><span data-stu-id="1f627-106">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="1f627-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="1f627-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="1f627-108">Версия /v1.0 этот интерфейс API переименовано в *groupSettings списка*.</span><span class="sxs-lookup"><span data-stu-id="1f627-108">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f627-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f627-109">Permissions</span></span>
<span data-ttu-id="1f627-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f627-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f627-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f627-112">Permission type</span></span>      | <span data-ttu-id="1f627-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f627-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f627-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f627-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1f627-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1f627-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1f627-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f627-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f627-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f627-117">Not supported.</span></span>    |
|<span data-ttu-id="1f627-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f627-118">Application</span></span> | <span data-ttu-id="1f627-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f627-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f627-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f627-120">HTTP request</span></span>
<span data-ttu-id="1f627-121"><!-- { "blockType": "ignored" } -->Список всей клиента или параметры группы</span><span class="sxs-lookup"><span data-stu-id="1f627-121"><!-- { "blockType": "ignored" } --> List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1f627-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f627-122">Optional query parameters</span></span>
<span data-ttu-id="1f627-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f627-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f627-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f627-124">Request headers</span></span>
| <span data-ttu-id="1f627-125">Имя</span><span class="sxs-lookup"><span data-stu-id="1f627-125">Name</span></span>      |<span data-ttu-id="1f627-126">Описание</span><span class="sxs-lookup"><span data-stu-id="1f627-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f627-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f627-127">Authorization</span></span>  | <span data-ttu-id="1f627-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f627-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f627-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f627-130">Request body</span></span>
<span data-ttu-id="1f627-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f627-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f627-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f627-132">Response</span></span>

<span data-ttu-id="1f627-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [directorySetting](../resources/directorysetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1f627-133">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f627-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1f627-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f627-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f627-135">Request</span></span>
<span data-ttu-id="1f627-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f627-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="1f627-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f627-137">Response</span></span>
<span data-ttu-id="1f627-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1f627-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
