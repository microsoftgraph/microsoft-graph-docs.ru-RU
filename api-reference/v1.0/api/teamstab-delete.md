---
title: Удалить вкладку с канала
description: 'Удаляет (отключит) вкладки с указанными в группе. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 672077e4b1ac383ca6e6bb415ff25639fb03dc08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917435"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="8d434-103">Удалить вкладку с канала</span><span class="sxs-lookup"><span data-stu-id="8d434-103">Delete tab from channel</span></span>



<span data-ttu-id="8d434-104">Удаляет (отключит) вкладки из указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8d434-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d434-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d434-105">Permissions</span></span>
<span data-ttu-id="8d434-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d434-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d434-108">Permission type</span></span>      | <span data-ttu-id="8d434-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d434-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d434-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d434-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d434-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d434-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d434-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d434-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d434-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d434-113">Not supported.</span></span>    |
|<span data-ttu-id="8d434-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d434-114">Application</span></span> | <span data-ttu-id="8d434-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d434-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="8d434-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="8d434-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8d434-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="8d434-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8d434-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d434-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d434-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d434-119">Request headers</span></span>
| <span data-ttu-id="8d434-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d434-120">Header</span></span>       | <span data-ttu-id="8d434-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d434-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d434-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d434-122">Authorization</span></span>  | <span data-ttu-id="8d434-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d434-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d434-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d434-125">Request body</span></span>
<span data-ttu-id="8d434-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d434-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d434-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d434-127">Response</span></span>

<span data-ttu-id="8d434-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8d434-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d434-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8d434-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8d434-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d434-131">Request</span></span>
<span data-ttu-id="8d434-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d434-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="8d434-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d434-133">Response</span></span>
<span data-ttu-id="8d434-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d434-134">The following is an example of the response.</span></span> <span data-ttu-id="8d434-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8d434-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8d434-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d434-136">All of the properties will be returned from an actual call.</span></span>
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
