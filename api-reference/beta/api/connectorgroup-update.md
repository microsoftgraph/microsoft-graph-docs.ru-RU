---
title: Обновление Коннекторграупс
description: Обновление свойств объекта коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: 9d6feec19552aeeebe51ba0fab07e805c6f4a2bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455767"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="55b65-103">Обновление Коннекторграупс</span><span class="sxs-lookup"><span data-stu-id="55b65-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55b65-104">Обновление свойств объекта коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="55b65-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55b65-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55b65-105">Permissions</span></span>
<span data-ttu-id="55b65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b65-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55b65-108">Permission type</span></span>      | <span data-ttu-id="55b65-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55b65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55b65-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55b65-110">Delegated (work or school account)</span></span> | <span data-ttu-id="55b65-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55b65-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55b65-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55b65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55b65-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b65-113">Not supported.</span></span>    |
|<span data-ttu-id="55b65-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55b65-114">Application</span></span> | <span data-ttu-id="55b65-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b65-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55b65-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55b65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="55b65-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55b65-117">Optional request headers</span></span>
| <span data-ttu-id="55b65-118">Имя</span><span class="sxs-lookup"><span data-stu-id="55b65-118">Name</span></span>       | <span data-ttu-id="55b65-119">Описание</span><span class="sxs-lookup"><span data-stu-id="55b65-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="55b65-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b65-120">Authorization</span></span>  | <span data-ttu-id="55b65-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="55b65-121">Bearer.</span></span> <span data-ttu-id="55b65-122">Обязательно</span><span class="sxs-lookup"><span data-stu-id="55b65-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="55b65-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55b65-123">Request body</span></span>
<span data-ttu-id="55b65-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="55b65-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="55b65-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b65-127">Property</span></span>     | <span data-ttu-id="55b65-128">Тип</span><span class="sxs-lookup"><span data-stu-id="55b65-128">Type</span></span>   |<span data-ttu-id="55b65-129">Описание</span><span class="sxs-lookup"><span data-stu-id="55b65-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55b65-130">Коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="55b65-130">connectorGroupType</span></span>|<span data-ttu-id="55b65-131">строка</span><span class="sxs-lookup"><span data-stu-id="55b65-131">string</span></span>| <span data-ttu-id="55b65-132">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="55b65-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="55b65-133">name</span><span class="sxs-lookup"><span data-stu-id="55b65-133">name</span></span>|<span data-ttu-id="55b65-134">String</span><span class="sxs-lookup"><span data-stu-id="55b65-134">String</span></span>|<span data-ttu-id="55b65-135">Имя Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="55b65-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="55b65-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="55b65-136">Response</span></span>

<span data-ttu-id="55b65-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55b65-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55b65-138">Пример</span><span class="sxs-lookup"><span data-stu-id="55b65-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55b65-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="55b65-139">Request</span></span>
<span data-ttu-id="55b65-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55b65-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="55b65-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55b65-141">Response</span></span>
<span data-ttu-id="55b65-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55b65-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
