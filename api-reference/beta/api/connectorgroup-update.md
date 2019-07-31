---
title: Обновление Коннекторграупс
description: Обновление свойств объекта коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dfc574c9028d5e810a92fd5de4b099d3109bf7ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943374"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="3b033-103">Обновление Коннекторграупс</span><span class="sxs-lookup"><span data-stu-id="3b033-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b033-104">Обновление свойств объекта коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="3b033-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b033-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b033-105">Permissions</span></span>
<span data-ttu-id="3b033-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b033-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b033-108">Permission type</span></span>      | <span data-ttu-id="3b033-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b033-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b033-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b033-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3b033-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b033-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b033-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b033-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b033-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b033-113">Not supported.</span></span>    |
|<span data-ttu-id="3b033-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b033-114">Application</span></span> | <span data-ttu-id="3b033-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b033-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b033-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b033-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3b033-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b033-117">Optional request headers</span></span>
| <span data-ttu-id="3b033-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3b033-118">Name</span></span>       | <span data-ttu-id="3b033-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3b033-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3b033-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b033-120">Authorization</span></span>  | <span data-ttu-id="3b033-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="3b033-121">Bearer.</span></span> <span data-ttu-id="3b033-122">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3b033-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b033-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b033-123">Request body</span></span>
<span data-ttu-id="3b033-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3b033-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b033-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b033-127">Property</span></span>     | <span data-ttu-id="3b033-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3b033-128">Type</span></span>   |<span data-ttu-id="3b033-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3b033-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b033-130">Коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="3b033-130">connectorGroupType</span></span>|<span data-ttu-id="3b033-131">string</span><span class="sxs-lookup"><span data-stu-id="3b033-131">string</span></span>| <span data-ttu-id="3b033-132">Возможные значения: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="3b033-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="3b033-133">name</span><span class="sxs-lookup"><span data-stu-id="3b033-133">name</span></span>|<span data-ttu-id="3b033-134">String</span><span class="sxs-lookup"><span data-stu-id="3b033-134">String</span></span>|<span data-ttu-id="3b033-135">Имя Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="3b033-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="3b033-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b033-136">Response</span></span>

<span data-ttu-id="3b033-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b033-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b033-138">Пример</span><span class="sxs-lookup"><span data-stu-id="3b033-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b033-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b033-139">Request</span></span>
<span data-ttu-id="3b033-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b033-140">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3b033-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b033-141">Response</span></span>
<span data-ttu-id="3b033-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b033-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
