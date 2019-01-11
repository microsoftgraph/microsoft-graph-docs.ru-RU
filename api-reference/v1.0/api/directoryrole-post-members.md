---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 11b06eac57d0850e8df5233bba47966f6b7932d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886641"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="a3482-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="a3482-103">Add directory role member</span></span>

<span data-ttu-id="a3482-104">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a3482-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3482-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3482-105">Permissions</span></span>
<span data-ttu-id="a3482-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3482-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3482-108">Permission type</span></span>      | <span data-ttu-id="a3482-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3482-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3482-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3482-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3482-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3482-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3482-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3482-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3482-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3482-113">Not supported.</span></span>    |
|<span data-ttu-id="a3482-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3482-114">Application</span></span> | <span data-ttu-id="a3482-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3482-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3482-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3482-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="a3482-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3482-117">Request headers</span></span>
| <span data-ttu-id="a3482-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a3482-118">Name</span></span>       | <span data-ttu-id="a3482-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a3482-119">Type</span></span> | <span data-ttu-id="a3482-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a3482-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a3482-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3482-121">Authorization</span></span>  | <span data-ttu-id="a3482-122">string</span><span class="sxs-lookup"><span data-stu-id="a3482-122">string</span></span>  | <span data-ttu-id="a3482-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3482-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a3482-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3482-125">Content-Type</span></span>  | <span data-ttu-id="a3482-126">строка</span><span class="sxs-lookup"><span data-stu-id="a3482-126">string</span></span>  | <span data-ttu-id="a3482-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3482-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3482-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3482-128">Request body</span></span>
<span data-ttu-id="a3482-129">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3482-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="a3482-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3482-130">Response</span></span>

<span data-ttu-id="a3482-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3482-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3482-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3482-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3482-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3482-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="a3482-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3482-134">Response</span></span>
<span data-ttu-id="a3482-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a3482-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
