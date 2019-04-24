---
title: Удаление элемента
description: С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: bda39ba1435d1368241db42a67b448fe178cef26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503116"
---
# <a name="remove-member"></a><span data-ttu-id="21dc1-104">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="21dc1-104">Remove member</span></span>
<span data-ttu-id="21dc1-p102">С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.</span><span class="sxs-lookup"><span data-stu-id="21dc1-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="21dc1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21dc1-107">Permissions</span></span>
<span data-ttu-id="21dc1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21dc1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21dc1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21dc1-110">Permission type</span></span>      | <span data-ttu-id="21dc1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21dc1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21dc1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21dc1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21dc1-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21dc1-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21dc1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21dc1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21dc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21dc1-115">Not supported.</span></span>    |
|<span data-ttu-id="21dc1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21dc1-116">Application</span></span> | <span data-ttu-id="21dc1-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21dc1-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="21dc1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21dc1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="21dc1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21dc1-119">Request headers</span></span>
| <span data-ttu-id="21dc1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="21dc1-120">Name</span></span>       | <span data-ttu-id="21dc1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="21dc1-121">Type</span></span> | <span data-ttu-id="21dc1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="21dc1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21dc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21dc1-123">Authorization</span></span>  | <span data-ttu-id="21dc1-124">string</span><span class="sxs-lookup"><span data-stu-id="21dc1-124">string</span></span>  | <span data-ttu-id="21dc1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21dc1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21dc1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21dc1-127">Request body</span></span>
<span data-ttu-id="21dc1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21dc1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21dc1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="21dc1-129">Response</span></span>
<span data-ttu-id="21dc1-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="21dc1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21dc1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="21dc1-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="21dc1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="21dc1-133">Request</span></span>
<span data-ttu-id="21dc1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21dc1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="21dc1-135">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="21dc1-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="21dc1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="21dc1-136">Response</span></span>
<span data-ttu-id="21dc1-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21dc1-137">The following is an example of the response.</span></span>
><span data-ttu-id="21dc1-138">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="21dc1-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21dc1-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21dc1-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
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
