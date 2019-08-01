---
title: Удаление вкладки из канала
description: 'Удаляет (открепляет) вкладку из указанного канала в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3dbba4b8996a86e8ff71d0dd115b0a00362e103f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027211"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="9091b-103">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="9091b-103">Delete tab from channel</span></span>



<span data-ttu-id="9091b-104">Удаляет (открепляет) вкладку из указанного [канала](../resources/channel.md) в [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9091b-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="9091b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9091b-105">Permissions</span></span>
<span data-ttu-id="9091b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9091b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9091b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9091b-108">Permission type</span></span>      | <span data-ttu-id="9091b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9091b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9091b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9091b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9091b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9091b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9091b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9091b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9091b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9091b-113">Not supported.</span></span>    |
|<span data-ttu-id="9091b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9091b-114">Application</span></span> | <span data-ttu-id="9091b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9091b-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="9091b-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9091b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9091b-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9091b-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9091b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9091b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9091b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9091b-119">Request headers</span></span>
| <span data-ttu-id="9091b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9091b-120">Header</span></span>       | <span data-ttu-id="9091b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9091b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9091b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9091b-122">Authorization</span></span>  | <span data-ttu-id="9091b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9091b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9091b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9091b-125">Request body</span></span>
<span data-ttu-id="9091b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9091b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9091b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9091b-127">Response</span></span>

<span data-ttu-id="9091b-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9091b-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9091b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9091b-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9091b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9091b-131">Request</span></span>
<span data-ttu-id="9091b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9091b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="9091b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9091b-133">Response</span></span>
<span data-ttu-id="9091b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9091b-134">The following is an example of the response.</span></span> <span data-ttu-id="9091b-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9091b-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9091b-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9091b-136">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
