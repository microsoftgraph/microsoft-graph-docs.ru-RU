---
title: Создание Коннекторграуп
description: Используйте этот API для создания нового Коннекторграуп.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 21cdb4ec3da098ed787c13a4b8c4c24244dd6c8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437310"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="eae1f-103">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="eae1f-103">Create connectorGroup</span></span>

<span data-ttu-id="eae1f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eae1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eae1f-105">Используйте этот API для создания нового Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="eae1f-105">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="eae1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eae1f-106">Permissions</span></span>
<span data-ttu-id="eae1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eae1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eae1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eae1f-109">Permission type</span></span>      | <span data-ttu-id="eae1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eae1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eae1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eae1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eae1f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eae1f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eae1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eae1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eae1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae1f-114">Not supported.</span></span>    |
|<span data-ttu-id="eae1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eae1f-115">Application</span></span> | <span data-ttu-id="eae1f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eae1f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eae1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eae1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="eae1f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eae1f-118">Request headers</span></span>
| <span data-ttu-id="eae1f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="eae1f-119">Name</span></span>       | <span data-ttu-id="eae1f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eae1f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eae1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eae1f-121">Authorization</span></span>  | <span data-ttu-id="eae1f-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="eae1f-122">Bearer.</span></span> <span data-ttu-id="eae1f-123">рекуриед</span><span class="sxs-lookup"><span data-stu-id="eae1f-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="eae1f-124">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="eae1f-124">Request body</span></span>
<span data-ttu-id="eae1f-125">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eae1f-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eae1f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="eae1f-126">Response</span></span>

<span data-ttu-id="eae1f-127">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eae1f-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eae1f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="eae1f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eae1f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="eae1f-129">Request</span></span>
<span data-ttu-id="eae1f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eae1f-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="eae1f-131">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eae1f-131">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eae1f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="eae1f-132">Response</span></span>
<span data-ttu-id="eae1f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eae1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
