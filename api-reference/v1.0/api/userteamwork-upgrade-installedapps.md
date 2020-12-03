---
title: 'Теамсаппинсталлатион: обновление'
description: Обновление установки приложения в личной области пользователя
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8b38ef1ab60dc2d38a52acaeabe0e2c5491d2d5a
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564081"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="5ea12-103">Теамсаппинсталлатион: обновление</span><span class="sxs-lookup"><span data-stu-id="5ea12-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="5ea12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ea12-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в личной области указанного [пользователя](../resources/user.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="5ea12-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea12-106">Permissions</span></span>

<span data-ttu-id="5ea12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ea12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea12-109">Permission type</span></span>      | <span data-ttu-id="5ea12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ea12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea12-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ea12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea12-112">Теамсаппинсталлатион. Реадвритеселффорусер, Теамсаппинсталлатион. Реадвритефорусер, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ea12-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="5ea12-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ea12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ea12-114">Not supported.</span></span>    |
|<span data-ttu-id="5ea12-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ea12-115">Application</span></span> | <span data-ttu-id="5ea12-116">Теамсаппинсталлатион. Реадвритеселффорусер. ALL, Теамсаппинсталлатион. Реадвритефорусер. ALL, TeamsAppInstallation. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ea12-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ea12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ea12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="5ea12-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ea12-118">Request headers</span></span>

| <span data-ttu-id="5ea12-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ea12-119">Header</span></span>       | <span data-ttu-id="5ea12-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5ea12-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ea12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ea12-121">Authorization</span></span>  | <span data-ttu-id="5ea12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ea12-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ea12-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ea12-124">Request body</span></span>

<span data-ttu-id="5ea12-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ea12-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ea12-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea12-126">Response</span></span>

<span data-ttu-id="5ea12-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5ea12-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea12-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5ea12-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea12-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ea12-130">Request</span></span>

<span data-ttu-id="5ea12-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ea12-131">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->

```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```

### <a name="response"></a><span data-ttu-id="5ea12-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea12-132">Response</span></span>

<span data-ttu-id="5ea12-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea12-133">The following is an example of the response.</span></span>

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
