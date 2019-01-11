---
title: Обновление приложения в группе
description: Обновляет установку приложения в группе
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 36ddc41e6c15def1c5570fc49c3b151c87a63421
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826602"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="24d89-103">Обновление приложения в группе</span><span class="sxs-lookup"><span data-stu-id="24d89-103">Upgrade an app in a team</span></span>



<span data-ttu-id="24d89-104">Обновляет [установки приложения](../resources/teamsappinstallation.md) в [группы](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="24d89-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="24d89-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24d89-105">Permissions</span></span>

<span data-ttu-id="24d89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d89-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24d89-108">Permission type</span></span>      | <span data-ttu-id="24d89-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24d89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24d89-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24d89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24d89-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d89-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="24d89-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24d89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24d89-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d89-113">Not supported.</span></span>    |
|<span data-ttu-id="24d89-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24d89-114">Application</span></span> | <span data-ttu-id="24d89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d89-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24d89-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24d89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="24d89-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24d89-117">Request headers</span></span>
| <span data-ttu-id="24d89-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24d89-118">Header</span></span>       | <span data-ttu-id="24d89-119">Значение</span><span class="sxs-lookup"><span data-stu-id="24d89-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24d89-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24d89-120">Authorization</span></span>  | <span data-ttu-id="24d89-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24d89-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24d89-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24d89-123">Request body</span></span>
<span data-ttu-id="24d89-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24d89-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24d89-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="24d89-125">Response</span></span>

<span data-ttu-id="24d89-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="24d89-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d89-128">Пример</span><span class="sxs-lookup"><span data-stu-id="24d89-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="24d89-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="24d89-129">Request</span></span>
<span data-ttu-id="24d89-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24d89-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="24d89-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="24d89-131">Response</span></span>
<span data-ttu-id="24d89-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24d89-132">The following is an example of the response.</span></span> 

><span data-ttu-id="24d89-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24d89-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
