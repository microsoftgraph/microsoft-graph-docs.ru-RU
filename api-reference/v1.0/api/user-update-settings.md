---
title: Обновление параметров
description: 'Обновление свойств объекта Settings. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eb739ebe4266dc61246fd39f1b4f053ab08a5a75
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573573"
---
# <a name="update-settings"></a><span data-ttu-id="a773a-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="a773a-103">Update settings</span></span>

<span data-ttu-id="a773a-104">Обновление свойств объекта [Settings](../resources/user-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="a773a-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="a773a-105">Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтения или политики Организации.</span><span class="sxs-lookup"><span data-stu-id="a773a-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="a773a-106">Чтобы получить текущие параметры пользователя, просмотрите [параметры текущей учетной записи пользователя](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="a773a-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a773a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a773a-107">Permissions</span></span>

<span data-ttu-id="a773a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a773a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a773a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a773a-110">Permission type</span></span>      | <span data-ttu-id="a773a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a773a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a773a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a773a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a773a-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a773a-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="a773a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a773a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a773a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a773a-115">Not supported.</span></span>    |
|<span data-ttu-id="a773a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a773a-116">Application</span></span> | <span data-ttu-id="a773a-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a773a-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a773a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a773a-118">HTTP request</span></span>

```http
PATCH /me/settings
```

<span data-ttu-id="a773a-119">Запрос с идентификатором пользователя или userPrincipalName доступен только пользователю или пользователем с разрешениями User. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="a773a-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="a773a-120">Чтобы узнать больше, ознакомьтесь [](/graph/permissions-reference)с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="a773a-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="a773a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a773a-121">Request headers</span></span>

| <span data-ttu-id="a773a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a773a-122">Header</span></span>       | <span data-ttu-id="a773a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a773a-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a773a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a773a-124">Authorization</span></span>  | <span data-ttu-id="a773a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a773a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a773a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a773a-127">Content-Type</span></span>  | <span data-ttu-id="a773a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a773a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a773a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a773a-129">Request body</span></span>

<span data-ttu-id="a773a-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a773a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a773a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a773a-133">Property</span></span>     | <span data-ttu-id="a773a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a773a-134">Type</span></span>   |<span data-ttu-id="a773a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a773a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a773a-136">Контрибутионтоконтентдисковеридисаблед</span><span class="sxs-lookup"><span data-stu-id="a773a-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="a773a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a773a-137">Boolean</span></span>|<span data-ttu-id="a773a-138">Установите значение true, чтобы запретить представителю доступ [](/graph/api/resources/insights-trending?view=graph-rest-beta) к API тенденций и отключить доступ к документам в Office delve для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a773a-138">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="a773a-139">Значение true также влияет на релевантность контента, отображаемого в Office 365, например, Рекомендуемые сайты в SharePoint Home и представление обнаружение в OneDrive для бизнеса содержат менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="a773a-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="a773a-140">Этот параметр отражает состояние элемента управления в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="a773a-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="a773a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a773a-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="a773a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a773a-142">Request</span></span>

<span data-ttu-id="a773a-143">Ниже приведен пример запроса на отказаться от участия пользователя в delve и отказаться от его участия в релевантности контента для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="a773a-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="a773a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a773a-144">Response</span></span>

<span data-ttu-id="a773a-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a773a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="a773a-148">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="a773a-148">Batch request</span></span>

<span data-ttu-id="a773a-149">Кроме того, можно отказаться от использования нескольких пользователей из delve и отказаться от их вклада в релевантность содержимого для всей Организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="a773a-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="a773a-150">Для получения дополнительных сведений см [Пакетная обработка JSON](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span><span class="sxs-lookup"><span data-stu-id="a773a-150">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="a773a-151">**Важно!** только члены группы ролей " [Управление организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) " могут обновлять нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="a773a-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



