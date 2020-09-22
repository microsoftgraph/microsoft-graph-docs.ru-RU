---
title: Удаление объекта Скопедролемембер
description: Удаление члена с областью ролей из единицы админстративе.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9e884d568e3bd7d41a3fb3659c2fd270161a92e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020371"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="0524b-103">Удаление объекта Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="0524b-103">Remove a scopedRoleMember</span></span>

<span data-ttu-id="0524b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0524b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0524b-105">Удаление члена с областью ролей из единицы админстративе.</span><span class="sxs-lookup"><span data-stu-id="0524b-105">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="0524b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0524b-106">Permissions</span></span>
<span data-ttu-id="0524b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0524b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0524b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0524b-109">Permission type</span></span>      | <span data-ttu-id="0524b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0524b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0524b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0524b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0524b-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0524b-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0524b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0524b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0524b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0524b-114">Not supported.</span></span>    |
|<span data-ttu-id="0524b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0524b-115">Application</span></span> | <span data-ttu-id="0524b-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0524b-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0524b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0524b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0524b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0524b-118">Request headers</span></span>
| <span data-ttu-id="0524b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0524b-119">Name</span></span>       | <span data-ttu-id="0524b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0524b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0524b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0524b-121">Authorization</span></span>  | <span data-ttu-id="0524b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0524b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0524b-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0524b-124">Request body</span></span>
<span data-ttu-id="0524b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0524b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0524b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0524b-126">Response</span></span>

<span data-ttu-id="0524b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0524b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0524b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0524b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0524b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0524b-130">Request</span></span>
<span data-ttu-id="0524b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0524b-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/scopedRoleMembers/{id}
```

---

##### <a name="response"></a><span data-ttu-id="0524b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0524b-132">Response</span></span>
<span data-ttu-id="0524b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0524b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
