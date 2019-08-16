---
title: Создание Унифиедролеассигнмент
description: Создание нового объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1ce6c7d99a3316bdb5c45780f41e181906ff76f7
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437694"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="91974-103">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="91974-103">Create unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91974-104">Создание нового объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="91974-104">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91974-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91974-105">Permissions</span></span>

<span data-ttu-id="91974-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91974-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91974-108">Permission type</span></span>                        | <span data-ttu-id="91974-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91974-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91974-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91974-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="91974-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="91974-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="91974-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91974-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91974-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91974-113">Not supported.</span></span> |
| <span data-ttu-id="91974-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91974-114">Application</span></span>                            | <span data-ttu-id="91974-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="91974-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="91974-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91974-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="91974-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91974-117">Request headers</span></span>

| <span data-ttu-id="91974-118">Имя</span><span class="sxs-lookup"><span data-stu-id="91974-118">Name</span></span>          | <span data-ttu-id="91974-119">Описание</span><span class="sxs-lookup"><span data-stu-id="91974-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="91974-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91974-120">Authorization</span></span> | <span data-ttu-id="91974-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="91974-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="91974-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91974-122">Request body</span></span>

<span data-ttu-id="91974-123">В тексте запроса добавьте представление объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91974-123">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="91974-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="91974-124">Response</span></span>

<span data-ttu-id="91974-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91974-125">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91974-126">Пример</span><span class="sxs-lookup"><span data-stu-id="91974-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="91974-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="91974-127">Request</span></span>

<span data-ttu-id="91974-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91974-128">The following is an example of the request.</span></span> <span data-ttu-id="91974-129">Обратите внимание на использование параметра Ролетемплатеид для Роледефинитионид.</span><span class="sxs-lookup"><span data-stu-id="91974-129">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="91974-130">Роледефинитионид может быть либо идентификатором шаблона на уровне службы, либо Роледефинитионид, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="91974-130">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "principalId":"a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "roleDefinitionId":"b0f54661-2d74-4c50-afa3-1ec803f12efe",
    "resourceScope":"/"
}
```

### <a name="response"></a><span data-ttu-id="91974-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="91974-131">Response</span></span>

<span data-ttu-id="91974-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91974-132">The following is an example of the response.</span></span>

> <span data-ttu-id="91974-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91974-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "resourceScope": "/",
    "roleDefinitionId": "b0f54661-2d74-4c50-afa3-1ec803f12efe"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->