---
title: Удалить вкладку с канала
description: 'Удаляет (отключит) вкладки с указанными в группе. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 59f3628cee3a65549a94a19ef8ad265d0d4a5397
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812609"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="82d24-103">Удалить вкладку с канала</span><span class="sxs-lookup"><span data-stu-id="82d24-103">Delete tab from channel</span></span>

> <span data-ttu-id="82d24-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82d24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82d24-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82d24-106">Удаляет (отключит) вкладки из указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="82d24-106">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="82d24-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82d24-107">Permissions</span></span>
<span data-ttu-id="82d24-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d24-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d24-110">Permission type</span></span>      | <span data-ttu-id="82d24-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82d24-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82d24-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d24-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82d24-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d24-115">Not supported.</span></span>    |
|<span data-ttu-id="82d24-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82d24-116">Application</span></span> | <span data-ttu-id="82d24-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d24-117">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="82d24-118">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="82d24-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="82d24-119">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="82d24-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="82d24-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d24-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="82d24-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82d24-121">Request headers</span></span>
| <span data-ttu-id="82d24-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82d24-122">Header</span></span>       | <span data-ttu-id="82d24-123">Значение</span><span class="sxs-lookup"><span data-stu-id="82d24-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82d24-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82d24-124">Authorization</span></span>  | <span data-ttu-id="82d24-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82d24-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82d24-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82d24-127">Request body</span></span>
<span data-ttu-id="82d24-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82d24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82d24-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d24-129">Response</span></span>

<span data-ttu-id="82d24-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="82d24-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82d24-132">Пример</span><span class="sxs-lookup"><span data-stu-id="82d24-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="82d24-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d24-133">Request</span></span>
<span data-ttu-id="82d24-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82d24-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="82d24-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="82d24-135">Response</span></span>
<span data-ttu-id="82d24-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="82d24-136">The following is an example of the response.</span></span> <span data-ttu-id="82d24-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="82d24-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="82d24-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d24-138">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
