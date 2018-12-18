---
title: Обновление параметров
description: 'Обновляет свойства объекта settings. '
author: dkershaw10
ms.openlocfilehash: 571acf47852e703ee3bb20bd0c37cc5736cc4f1f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320253"
---
# <a name="update-settings"></a><span data-ttu-id="16e81-103">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="16e81-103">Update settings</span></span>

<span data-ttu-id="16e81-104">Обновляет свойства объекта [settings](../resources/user-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="16e81-104">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="16e81-105">Пользователи в той же организации могут иметь различные параметры на основе их приоритета или политики организации.</span><span class="sxs-lookup"><span data-stu-id="16e81-105">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="16e81-106">Для получения текущих параметров пользователя, просмотрите [параметры текущего пользователя](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="16e81-106">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="16e81-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16e81-107">Permissions</span></span>

<span data-ttu-id="16e81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16e81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16e81-110">Permission type</span></span>      | <span data-ttu-id="16e81-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16e81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16e81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16e81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="16e81-113">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e81-113">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="16e81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16e81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16e81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e81-115">Not supported.</span></span>    |
|<span data-ttu-id="16e81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16e81-116">Application</span></span> | <span data-ttu-id="16e81-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e81-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16e81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16e81-118">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

<span data-ttu-id="16e81-119">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="16e81-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="16e81-120">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="16e81-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="16e81-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16e81-121">Request headers</span></span>

| <span data-ttu-id="16e81-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16e81-122">Header</span></span>       | <span data-ttu-id="16e81-123">Значение</span><span class="sxs-lookup"><span data-stu-id="16e81-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="16e81-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16e81-124">Authorization</span></span>  | <span data-ttu-id="16e81-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16e81-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="16e81-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="16e81-127">Content-Type</span></span>  | <span data-ttu-id="16e81-128">application/json</span><span class="sxs-lookup"><span data-stu-id="16e81-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="16e81-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16e81-129">Request body</span></span>

<span data-ttu-id="16e81-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="16e81-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="16e81-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e81-133">Property</span></span>     | <span data-ttu-id="16e81-134">Тип</span><span class="sxs-lookup"><span data-stu-id="16e81-134">Type</span></span>   |<span data-ttu-id="16e81-135">Описание</span><span class="sxs-lookup"><span data-stu-id="16e81-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16e81-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="16e81-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="16e81-137">Boolean.</span><span class="sxs-lookup"><span data-stu-id="16e81-137">Boolean</span></span>|<span data-ttu-id="16e81-138">Параметр имеет значение true отключить делегированный доступ для [тенденций](/graph/api/resources/insights-trending?view=graph-rest-beta) API и отключать доступ к документам в углубимся Office для пользователя.</span><span class="sxs-lookup"><span data-stu-id="16e81-138">Set to true do disable delegate access to the [Trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="16e81-139">Настройка значение "true" также влияет на соответствие содержимого, отображаемые в Office 365 —, предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса Показать менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="16e81-139">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="16e81-140">Этот параметр отражает состояние элемента управления в [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="16e81-140">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="16e81-141">Пример</span><span class="sxs-lookup"><span data-stu-id="16e81-141">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="16e81-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="16e81-142">Request</span></span>

<span data-ttu-id="16e81-143">Ниже приведен пример запроса по отказаться пользователя из Delve и отключить его вклад в контента релевантности для всей организации.</span><span class="sxs-lookup"><span data-stu-id="16e81-143">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="16e81-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="16e81-144">Response</span></span>

<span data-ttu-id="16e81-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16e81-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="16e81-148">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="16e81-148">Batch request</span></span>

<span data-ttu-id="16e81-149">Можно также отказаться несколько пользователей из Delve и отключить их влияние на контента релевантности для всей организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="16e81-149">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="16e81-150">Для получения дополнительных сведений см [пакетные JSON](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span><span class="sxs-lookup"><span data-stu-id="16e81-150">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="16e81-151">**Важно**: только для членов группы ролей [Управления организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) можно обновить несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="16e81-151">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



