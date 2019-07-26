---
title: 'Теамсаппинсталлатион: обновление'
description: Обновление установки приложения в личной области пользователя
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7461c6e320ffcacc0d26ccffe90681ab6215db15
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908539"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="9719e-103">Теамсаппинсталлатион: обновление</span><span class="sxs-lookup"><span data-stu-id="9719e-103">teamsAppInstallation: upgrade</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9719e-104">Обновление [установки приложения](../resources/teamsappinstallation.md) в личной области указанного [пользователя](../resources/user.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="9719e-104">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="9719e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9719e-105">Permissions</span></span>

<span data-ttu-id="9719e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9719e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9719e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9719e-108">Permission type</span></span>      | <span data-ttu-id="9719e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9719e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9719e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9719e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9719e-111">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9719e-111">User.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="9719e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9719e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9719e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9719e-113">Not supported.</span></span>    |
|<span data-ttu-id="9719e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9719e-114">Application</span></span> | <span data-ttu-id="9719e-115">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9719e-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9719e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9719e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="9719e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9719e-117">Request headers</span></span>

| <span data-ttu-id="9719e-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9719e-118">Header</span></span>       | <span data-ttu-id="9719e-119">Значение</span><span class="sxs-lookup"><span data-stu-id="9719e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9719e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9719e-120">Authorization</span></span>  | <span data-ttu-id="9719e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9719e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9719e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9719e-123">Request body</span></span>

<span data-ttu-id="9719e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9719e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9719e-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="9719e-125">Response</span></span>

<span data-ttu-id="9719e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9719e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9719e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9719e-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="9719e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9719e-129">Request</span></span>

<span data-ttu-id="9719e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9719e-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

### <a name="response"></a><span data-ttu-id="9719e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9719e-131">Response</span></span>

<span data-ttu-id="9719e-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9719e-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
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
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
