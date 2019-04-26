---
title: Создание Коннекторграуп
description: Используйте этот API для создания нового Коннекторграуп.
localization_priority: Normal
ms.openlocfilehash: 90b3d0cdbdd02876e1dfaf3d6743f6dac2199202
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327682"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="cbcda-103">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="cbcda-103">Create connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbcda-104">Используйте этот API для создания нового Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="cbcda-104">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="cbcda-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbcda-105">Permissions</span></span>
<span data-ttu-id="cbcda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbcda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbcda-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbcda-108">Permission type</span></span>      | <span data-ttu-id="cbcda-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbcda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbcda-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbcda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cbcda-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cbcda-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cbcda-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbcda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbcda-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbcda-113">Not supported.</span></span>    |
|<span data-ttu-id="cbcda-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="cbcda-114">Application</span></span> | <span data-ttu-id="cbcda-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbcda-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbcda-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbcda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="cbcda-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbcda-117">Request headers</span></span>
| <span data-ttu-id="cbcda-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cbcda-118">Name</span></span>       | <span data-ttu-id="cbcda-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cbcda-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cbcda-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbcda-120">Authorization</span></span>  | <span data-ttu-id="cbcda-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="cbcda-121">Bearer.</span></span> <span data-ttu-id="cbcda-122">Рекуриед</span><span class="sxs-lookup"><span data-stu-id="cbcda-122">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbcda-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cbcda-123">Request body</span></span>
<span data-ttu-id="cbcda-124">В тексте запроса добавьте представление объекта [Коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbcda-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cbcda-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbcda-125">Response</span></span>

<span data-ttu-id="cbcda-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbcda-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbcda-127">Пример</span><span class="sxs-lookup"><span data-stu-id="cbcda-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbcda-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbcda-128">Request</span></span>
<span data-ttu-id="cbcda-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbcda-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="cbcda-130">В тексте запроса добавьте представление объекта [Коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbcda-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cbcda-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbcda-131">Response</span></span>
<span data-ttu-id="cbcda-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbcda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
