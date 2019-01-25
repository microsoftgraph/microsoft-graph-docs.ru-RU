---
title: Обновление параметров
description: 'Обновляет свойства объекта settings. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d21d7fb26945e4a46fdf877bb5911aba0621ce3b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508764"
---
# <a name="update-settings"></a><span data-ttu-id="af6de-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="af6de-103">Update settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af6de-104">Обновляет свойства объекта [settings](../resources/user-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="af6de-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="af6de-105">Пользователи в той же организации могут иметь различные параметры на основе их приоритета или политики организации.</span><span class="sxs-lookup"><span data-stu-id="af6de-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="af6de-106">Для получения текущих параметров пользователя, просмотрите [параметры текущего пользователя](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="af6de-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="af6de-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af6de-107">Permissions</span></span>

<span data-ttu-id="af6de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af6de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af6de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af6de-110">Permission type</span></span>      | <span data-ttu-id="af6de-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af6de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af6de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af6de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="af6de-113">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af6de-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="af6de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af6de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af6de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af6de-115">Not supported.</span></span>    |
|<span data-ttu-id="af6de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af6de-116">Application</span></span> | <span data-ttu-id="af6de-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af6de-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af6de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af6de-118">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

<span data-ttu-id="af6de-119">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="af6de-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="af6de-120">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="af6de-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="af6de-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af6de-121">Request headers</span></span>

| <span data-ttu-id="af6de-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af6de-122">Header</span></span>       | <span data-ttu-id="af6de-123">Значение</span><span class="sxs-lookup"><span data-stu-id="af6de-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="af6de-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af6de-124">Authorization</span></span>  | <span data-ttu-id="af6de-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af6de-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af6de-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af6de-127">Content-Type</span></span>  | <span data-ttu-id="af6de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="af6de-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af6de-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af6de-129">Request body</span></span>

<span data-ttu-id="af6de-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="af6de-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="af6de-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="af6de-133">Property</span></span>     | <span data-ttu-id="af6de-134">Тип</span><span class="sxs-lookup"><span data-stu-id="af6de-134">Type</span></span>   |<span data-ttu-id="af6de-135">Описание</span><span class="sxs-lookup"><span data-stu-id="af6de-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af6de-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="af6de-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="af6de-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="af6de-137">Boolean</span></span>|<span data-ttu-id="af6de-138">Параметр имеет значение true отключить делегированный доступ для [тенденций](../resources/insights-trending.md) API и отключать доступ к документам в углубимся Office для пользователя.</span><span class="sxs-lookup"><span data-stu-id="af6de-138">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="af6de-139">Настройка значение "true" также влияет на соответствие содержимого, отображаемые в Office 365 —, предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса Показать менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="af6de-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="af6de-140">Этот параметр отражает состояние элемента управления в [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="af6de-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="af6de-141">Пример</span><span class="sxs-lookup"><span data-stu-id="af6de-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="af6de-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="af6de-142">Request</span></span>

<span data-ttu-id="af6de-143">Ниже приведен пример запроса по отказаться пользователя из Delve и отключить его вклад в контента релевантности для всей организации.</span><span class="sxs-lookup"><span data-stu-id="af6de-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="af6de-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="af6de-144">Response</span></span>

<span data-ttu-id="af6de-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="af6de-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="af6de-148">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="af6de-148">Batch request</span></span>

<span data-ttu-id="af6de-149">Можно также отказаться несколько пользователей из Delve и отключить их влияние на контента релевантности для всей организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="af6de-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="af6de-150">Для получения дополнительных сведений см [пакетные JSON](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="af6de-150">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="af6de-151">**Важно**: только для членов группы ролей [Управления организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) можно обновить несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="af6de-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
