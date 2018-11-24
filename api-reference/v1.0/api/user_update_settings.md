# <a name="update-settings"></a><span data-ttu-id="7b4d5-101">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="7b4d5-101">Update settings</span></span>

<span data-ttu-id="7b4d5-102">Обновляет свойства объекта [settings](../resources/user_settings.md) .</span><span class="sxs-lookup"><span data-stu-id="7b4d5-102">Update the properties of the [settings](../resources/user_settings.md) object.</span></span> <span data-ttu-id="7b4d5-103">Пользователи в той же организации могут иметь различные параметры на основе их приоритета или политики организации.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-103">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="7b4d5-104">Для получения текущих параметров пользователя, просмотрите [параметры текущего пользователя](user_get_settings.md).</span><span class="sxs-lookup"><span data-stu-id="7b4d5-104">To get the user current settings, see [current user settings](user_get_settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="7b4d5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b4d5-105">Permissions</span></span>

<span data-ttu-id="7b4d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b4d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b4d5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b4d5-108">Permission type</span></span>      | <span data-ttu-id="7b4d5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b4d5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b4d5-111">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4d5-111">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="7b4d5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b4d5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-113">Not supported.</span></span>    |
|<span data-ttu-id="7b4d5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b4d5-114">Application</span></span> | <span data-ttu-id="7b4d5-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b4d5-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b4d5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b4d5-116">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

<span data-ttu-id="7b4d5-117">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="7b4d5-118">[Для получения дополнительных сведений см.](../../../concepts/permissions_reference.md)</span><span class="sxs-lookup"><span data-stu-id="7b4d5-118">To learn more, see [Permissions](../../../concepts/permissions_reference.md).</span></span> 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="7b4d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b4d5-119">Request headers</span></span>

| <span data-ttu-id="7b4d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b4d5-120">Header</span></span>       | <span data-ttu-id="7b4d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b4d5-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7b4d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b4d5-122">Authorization</span></span>  | <span data-ttu-id="7b4d5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b4d5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b4d5-125">Content-Type</span></span>  | <span data-ttu-id="7b4d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b4d5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b4d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b4d5-127">Request body</span></span>

<span data-ttu-id="7b4d5-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7b4d5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b4d5-131">Property</span></span>     | <span data-ttu-id="7b4d5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7b4d5-132">Type</span></span>   |<span data-ttu-id="7b4d5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7b4d5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b4d5-134">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="7b4d5-134">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="7b4d5-135">Логический</span><span class="sxs-lookup"><span data-stu-id="7b4d5-135">Boolean</span></span>|<span data-ttu-id="7b4d5-136">Параметр имеет значение true отключить делегированный доступ для [тенденций](../../beta/resources/insights_trending.md) API и отключать доступ к документам в углубимся Office для пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-136">Set to true do disable delegate access to the [Trending](../../beta/resources/insights_trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="7b4d5-137">Настройка значение "true" также влияет на соответствие содержимого, отображаемые в Office 365 —, предлагаемые сайты в Домашняя страница SharePoint и представления обнаружения в OneDrive для бизнеса Показать менее релевантные результаты.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-137">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="7b4d5-138">Этот параметр отражает состояние элемента управления в [Углубимся Office](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="7b4d5-138">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="7b4d5-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7b4d5-139">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="7b4d5-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b4d5-140">Request</span></span>

<span data-ttu-id="7b4d5-141">Ниже приведен пример запроса по отказаться пользователя из Delve и отключить его вклад в контента релевантности для всей организации.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-141">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="7b4d5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="7b4d5-142">Response</span></span>

<span data-ttu-id="7b4d5-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7b4d5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="7b4d5-146">Пакетный запрос</span><span class="sxs-lookup"><span data-stu-id="7b4d5-146">Batch request</span></span>

<span data-ttu-id="7b4d5-147">Можно также отказаться несколько пользователей из Delve и отключить их влияние на контента релевантности для всей организации с помощью пакетного запроса.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-147">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="7b4d5-148">Для получения дополнительных сведений см [пакетные JSON](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span><span class="sxs-lookup"><span data-stu-id="7b4d5-148">To learn more, see [JSON batching](https://developer.microsoft.com/graph/docs/concepts/json_batching).</span></span>

<span data-ttu-id="7b4d5-149">**Важно**: только для членов группы ролей [Управления организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) можно обновить несколько пользователей.</span><span class="sxs-lookup"><span data-stu-id="7b4d5-149">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 



