---
title: Обновление параметров
description: 'Обновляет свойства объекта settings. '
ms.openlocfilehash: 53b5fb2ce37aa9d80466face5ec03d1b54e87c09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081630"
---
# <a name="update-settings"></a><span data-ttu-id="17472-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="17472-103">Update settings</span></span>

> <span data-ttu-id="17472-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17472-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17472-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17472-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17472-106">Обновляет свойства объекта [settings](../resources/user-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="17472-106">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="17472-107">Пользователи в той же организации могут иметь различные параметры на основе их приоритета или политики организации.</span><span class="sxs-lookup"><span data-stu-id="17472-107">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="17472-108">Для получения текущих параметров пользователя, просмотрите [параметры текущего пользователя](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="17472-108">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="17472-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17472-109">Permissions</span></span>

<span data-ttu-id="17472-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17472-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17472-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17472-112">Permission type</span></span>      | <span data-ttu-id="17472-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17472-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17472-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17472-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17472-115">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17472-115">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="17472-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17472-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17472-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17472-117">Not supported.</span></span>    |
|<span data-ttu-id="17472-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17472-118">Application</span></span> | <span data-ttu-id="17472-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17472-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17472-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17472-120">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

<span data-ttu-id="17472-121">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="17472-121">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="17472-122">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="17472-122">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="17472-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17472-123">Request headers</span></span>

| <span data-ttu-id="17472-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17472-124">Header</span></span>       | <span data-ttu-id="17472-125">Значение</span><span class="sxs-lookup"><span data-stu-id="17472-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="17472-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17472-126">Authorization</span></span>  | <span data-ttu-id="17472-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17472-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17472-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17472-129">Content-Type</span></span>  | <span data-ttu-id="17472-130">application/json</span><span class="sxs-lookup"><span data-stu-id="17472-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17472-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17472-131">Request body</span></span>

<span data-ttu-id="17472-p106">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="17472-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17472-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="17472-135">Property</span></span>     | <span data-ttu-id="17472-136">Тип</span><span class="sxs-lookup"><span data-stu-id="17472-136">Type</span></span>   |<span data-ttu-id="17472-137">Description</span><span class="sxs-lookup"><span data-stu-id="17472-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17472-138">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="17472-138">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="17472-139">Логический</span><span class="sxs-lookup"><span data-stu-id="17472-139">Boolean</span></span>|<span data-ttu-id="17472-140">Параметр имеет значение true отключить делегированный доступ для [тенденций](../resources/insights-trending.md) API и отключать доступ к документам в углубимся Office для пользователя.</span><span class="sxs-lookup"><span data-stu-id="17472-140">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="17472-141">Настройка значение "true" также влияет на соответствие содержимого, отображаемые в Office 365 —, предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса Показать менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="17472-141">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="17472-142">Этот параметр отражает состояние элемента управления в [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="17472-142">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="17472-143">Пример</span><span class="sxs-lookup"><span data-stu-id="17472-143">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="17472-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="17472-144">Request</span></span>

<span data-ttu-id="17472-145">Ниже приведен пример запроса по отказаться пользователя из Delve и отключить его вклад в контента релевантности для всей организации.</span><span class="sxs-lookup"><span data-stu-id="17472-145">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="17472-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="17472-146">Response</span></span>

<span data-ttu-id="17472-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="17472-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="17472-150">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="17472-150">Batch request</span></span>

<span data-ttu-id="17472-151">Можно также отказаться несколько пользователей из Delve и отключить их влияние на контента релевантности для всей организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="17472-151">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="17472-152">Для получения дополнительных сведений см [пакетные JSON](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="17472-152">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="17472-153">**Важно**: только для членов группы ролей [Управления организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) можно обновить несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="17472-153">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


