---
title: Создание connectorGroup
description: Используйте этот интерфейс API для создания нового connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 65fe6dd901de6238c450b4896b37d56fa8ea602f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824299"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="81f6c-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="81f6c-103">Create connectorGroup</span></span>

> <span data-ttu-id="81f6c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81f6c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81f6c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81f6c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81f6c-106">Используйте этот интерфейс API для создания нового connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="81f6c-106">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="81f6c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81f6c-107">Permissions</span></span>
<span data-ttu-id="81f6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81f6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81f6c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81f6c-110">Permission type</span></span>      | <span data-ttu-id="81f6c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81f6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81f6c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81f6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="81f6c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81f6c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81f6c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81f6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81f6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81f6c-115">Not supported.</span></span>    |
|<span data-ttu-id="81f6c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81f6c-116">Application</span></span> | <span data-ttu-id="81f6c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f6c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81f6c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81f6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="81f6c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81f6c-119">Request headers</span></span>
| <span data-ttu-id="81f6c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="81f6c-120">Name</span></span>       | <span data-ttu-id="81f6c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="81f6c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81f6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81f6c-122">Authorization</span></span>  | <span data-ttu-id="81f6c-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="81f6c-123">Bearer.</span></span> <span data-ttu-id="81f6c-124">Ли</span><span class="sxs-lookup"><span data-stu-id="81f6c-124">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f6c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81f6c-125">Request body</span></span>
<span data-ttu-id="81f6c-126">В тексте запроса укажите представление JSON объекта [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="81f6c-126">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81f6c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f6c-127">Response</span></span>

<span data-ttu-id="81f6c-128">Успешно завершена, этот метод возвращает `201 Created` объект [connectorGroup](../resources/connectorgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81f6c-128">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81f6c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="81f6c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81f6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="81f6c-130">Request</span></span>
<span data-ttu-id="81f6c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81f6c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="81f6c-132">В тексте запроса укажите представление JSON объекта [connectorGroup](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="81f6c-132">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="81f6c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f6c-133">Response</span></span>
<span data-ttu-id="81f6c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81f6c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
