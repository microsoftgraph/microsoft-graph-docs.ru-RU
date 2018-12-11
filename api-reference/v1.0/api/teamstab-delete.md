---
title: Удалить вкладку с канала
description: 'Удаляет (отключит) вкладки с указанными в группе. '
ms.openlocfilehash: 2b132d2d127ff665b1cf408f38221e8bda09c166
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222340"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="bfa5e-103">Удалить вкладку с канала</span><span class="sxs-lookup"><span data-stu-id="bfa5e-103">Delete tab from channel</span></span>



<span data-ttu-id="bfa5e-104">Удаляет (отключит) вкладки из указанного [канала](../resources/channel.md) в пределах [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="bfa5e-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="bfa5e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfa5e-105">Permissions</span></span>
<span data-ttu-id="bfa5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfa5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfa5e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfa5e-108">Permission type</span></span>      | <span data-ttu-id="bfa5e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfa5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfa5e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfa5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfa5e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa5e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bfa5e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfa5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfa5e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-113">Not supported.</span></span>    |
|<span data-ttu-id="bfa5e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfa5e-114">Application</span></span> | <span data-ttu-id="bfa5e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa5e-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="bfa5e-116">**Примечание**: этот интерфейс API поддерживает разрешениями администратора.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bfa5e-117">Глобальных администраторов и администраторов службы группами Майкрософт могут получить доступ к группам будут недоступны, они не должна быть членом.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bfa5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfa5e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bfa5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfa5e-119">Request headers</span></span>
| <span data-ttu-id="bfa5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfa5e-120">Header</span></span>       | <span data-ttu-id="bfa5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bfa5e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfa5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfa5e-122">Authorization</span></span>  | <span data-ttu-id="bfa5e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfa5e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfa5e-125">Request body</span></span>
<span data-ttu-id="bfa5e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfa5e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfa5e-127">Response</span></span>

<span data-ttu-id="bfa5e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfa5e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bfa5e-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bfa5e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfa5e-131">Request</span></span>
<span data-ttu-id="bfa5e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="bfa5e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfa5e-133">Response</span></span>
<span data-ttu-id="bfa5e-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-134">The following is an example of the response.</span></span> <span data-ttu-id="bfa5e-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bfa5e-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfa5e-136">All of the properties will be returned from an actual call.</span></span>
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
