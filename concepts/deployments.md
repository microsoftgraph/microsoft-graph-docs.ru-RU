---
title: Национальные облачные развертывания
description: В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах. Эти национальные версии представляют собой изолированные в логических сетях физические экземпляры корпоративных облачных служб Майкрософт, которые находятся в географических границах определенных стран и обслуживаются местным персоналом. Дополнительные сведения см. в статье "Национальные облака Майкрософт".
ms.openlocfilehash: b0f2ab257773faa14fe59566992bb1ed0dd77959
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092570"
---
# <a name="national-cloud-deployments"></a><span data-ttu-id="e19a9-105">Национальные облачные развертывания</span><span class="sxs-lookup"><span data-stu-id="e19a9-105">National cloud deployments</span></span>


<span data-ttu-id="e19a9-106">В дополнение к нашей глобальной сети центров обработки данных облачные службы Майкрософт доступны в трех отдельных национальных облачных службах.</span><span class="sxs-lookup"><span data-stu-id="e19a9-106">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="e19a9-107">Эти национальные версии представляют собой изолированные в логических сетях физические экземпляры корпоративных облачных служб Майкрософт, которые находятся в географических границах определенных стран и обслуживаются местным персоналом.</span><span class="sxs-lookup"><span data-stu-id="e19a9-107">These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel.</span></span> <span data-ttu-id="e19a9-108">Дополнительные сведения см. в статье [Национальные облака Майкрософт](https://www.microsoft.com/ru-RU/TrustCenter/CloudServices/NationalCloud).</span><span class="sxs-lookup"><span data-stu-id="e19a9-108">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/ru-RU/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="e19a9-109">Существующие национальные облака:</span><span class="sxs-lookup"><span data-stu-id="e19a9-109">Current national clouds include:</span></span>

- <span data-ttu-id="e19a9-110">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e19a9-110">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="e19a9-111">Microsoft Cloud для Германии</span><span class="sxs-lookup"><span data-stu-id="e19a9-111">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="e19a9-112">Службы Azure и Office 365 под управлением компании 21Vianet в Китае</span><span class="sxs-lookup"><span data-stu-id="e19a9-112">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="e19a9-113">В этой статье приведены сведения о различных национальных облачных развертываниях Microsoft Graph, а также о возможностях, доступных разработчикам в каждом развертывании.</span><span class="sxs-lookup"><span data-stu-id="e19a9-113">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="e19a9-114">Корневые конечные точки служб Microsoft Graph и Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="e19a9-114">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="e19a9-115">В таблице ниже показаны конечные корневые точки службы Microsoft Graph и песочницы Microsoft Graph в каждом национальном облаке.</span><span class="sxs-lookup"><span data-stu-id="e19a9-115">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="e19a9-116">Национальное облако</span><span class="sxs-lookup"><span data-stu-id="e19a9-116">National Cloud</span></span> | <span data-ttu-id="e19a9-117">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e19a9-117">Microsoft Graph</span></span> | <span data-ttu-id="e19a9-118">Песочница Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e19a9-118">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="e19a9-119">Microsoft Graph для Китая под управлением 21Vianet</span><span class="sxs-lookup"><span data-stu-id="e19a9-119">Microsoft Graph China operated by 21Vianet</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="e19a9-120">Microsoft Graph для Германии</span><span class="sxs-lookup"><span data-stu-id="e19a9-120">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="e19a9-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e19a9-121">Not supported.</span></span> |
| <span data-ttu-id="e19a9-122">Microsoft Graph для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="e19a9-122">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="e19a9-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e19a9-123">Not supported.</span></span> |
| <span data-ttu-id="e19a9-124">Глобальная служба Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e19a9-124">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="e19a9-125">**Примечание.** Приложения могут получать доступ к данным организации только через конечные точки национальных облачных служб.</span><span class="sxs-lookup"><span data-stu-id="e19a9-125">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="e19a9-126">Это означает, что доступны только данные клиентов, зарегистрированных в определенном национальном облаке.</span><span class="sxs-lookup"><span data-stu-id="e19a9-126">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="e19a9-127">Приложения, которые с помощью Microsoft Graph пытаются получить доступ к данным потребителей, связанным с личными учетными записями Майкрософт, должны использовать глобальную службу (https://graph.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e19a9-127">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="e19a9-128">Маркеры доступа, приобретенные для национального облачного развертывания, не могут быть заменены маркерами, приобретенными для глобальный службы.</span><span class="sxs-lookup"><span data-stu-id="e19a9-128">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="e19a9-129">Конечные точки Azure AD OpenID Connect и OAuth2.0</span><span class="sxs-lookup"><span data-stu-id="e19a9-129">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="e19a9-130">В таблице ниже указаны базовые URL-адреса конечных точек Azure Active Directory (Azure AD), которые позволяют получить маркеры для вызова Microsoft Graph в каждом национальном облаке.</span><span class="sxs-lookup"><span data-stu-id="e19a9-130">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="e19a9-131">Национальное облако</span><span class="sxs-lookup"><span data-stu-id="e19a9-131">National Cloud</span></span> | <span data-ttu-id="e19a9-132">Корневая конечная точка Azure AD</span><span class="sxs-lookup"><span data-stu-id="e19a9-132">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="e19a9-133">Azure AD для Китая под управлением 21Vianet</span><span class="sxs-lookup"><span data-stu-id="e19a9-133">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="e19a9-134">Azure AD для Германии</span><span class="sxs-lookup"><span data-stu-id="e19a9-134">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="e19a9-135">Azure AD для государственных организаций США</span><span class="sxs-lookup"><span data-stu-id="e19a9-135">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="e19a9-136">Azure AD (глобальная служба)</span><span class="sxs-lookup"><span data-stu-id="e19a9-136">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="e19a9-p104">Запросы к конечным точкам авторизации или маркеров Azure AD могут быть созданы с помощью соответствующего базового URL-адреса для определенной страны или региона. Пример для Германии:</span><span class="sxs-lookup"><span data-stu-id="e19a9-p104">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="e19a9-139">Общая конечная точка авторизации: https://login.microsoftonline.de/common/oauth2/authorize.</span><span class="sxs-lookup"><span data-stu-id="e19a9-139">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="e19a9-140">Общая конечная точка маркера: https://login.microsoftonline.de/common/oauth2/token.</span><span class="sxs-lookup"><span data-stu-id="e19a9-140">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="e19a9-p105">Конечные точки для определенного клиента создаются путем замены элемента "common" в указанных выше URL-адресах идентификатором или проверенным доменом клиента. Выбор между общими конечными точками и точками для определенного клиента зависит от требований вашего приложения и процедуры проверки подлинности, используемой для получения маркеров. Дополнительные сведения о маркерах доступа Azure AD и Microsoft Graph см. в статье [Получение маркеров проверки подлинности](./auth-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e19a9-p105">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth-overview.md).</span></span>

> <span data-ttu-id="e19a9-144">**Примечание.** [Конечные точки авторизации и маркеров Azure AD версии 2.0](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-appmodel-v2-overview/) доступны только в глобальной службе и не могут использоваться с национальными облачными развертываниями.</span><span class="sxs-lookup"><span data-stu-id="e19a9-144">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/ru-RU/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="e19a9-145">Поддерживаемые функции</span><span class="sxs-lookup"><span data-stu-id="e19a9-145">Supported features</span></span>

<span data-ttu-id="e19a9-146">Указанные ниже компоненты Microsoft Graph (в конечной точке `/v1.0`) доступны во всех национальных облачных развертываниях, за исключением отмеченных.</span><span class="sxs-lookup"><span data-stu-id="e19a9-146">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e19a9-147">Пользователи</span><span class="sxs-lookup"><span data-stu-id="e19a9-147">Users</span></span>
* <span data-ttu-id="e19a9-148">Группы</span><span class="sxs-lookup"><span data-stu-id="e19a9-148">Groups</span></span>
* <span data-ttu-id="e19a9-149">Excel (ограничена поддержка службы Microsoft Graph под управлением 21Vianet в Китае)</span><span class="sxs-lookup"><span data-stu-id="e19a9-149">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e19a9-150">OneDrive (ограничена поддержка службы Microsoft Graph под управлением 21Vianet в Китае)</span><span class="sxs-lookup"><span data-stu-id="e19a9-150">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e19a9-151">Почта</span><span class="sxs-lookup"><span data-stu-id="e19a9-151">Outlook Mail</span></span>
* <span data-ttu-id="e19a9-152">Календарь Outlook</span><span class="sxs-lookup"><span data-stu-id="e19a9-152">Outlook Calendar</span></span>
* <span data-ttu-id="e19a9-153">Личные контакты</span><span class="sxs-lookup"><span data-stu-id="e19a9-153">Personal Contacts</span></span> 
* <span data-ttu-id="e19a9-154">SharePoint (ограничена поддержка службы Microsoft Graph под управлением 21Vianet в Китае)</span><span class="sxs-lookup"><span data-stu-id="e19a9-154">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e19a9-155">Разностный запрос (поддержка различных ресурсов зависит от национального облачного развертывания)</span><span class="sxs-lookup"><span data-stu-id="e19a9-155">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="e19a9-156">Веб-перехватчики (поддержка различных ресурсов зависит от национального облачного развертывания)</span><span class="sxs-lookup"><span data-stu-id="e19a9-156">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="e19a9-157">Указанные ниже дополнительные компоненты Microsoft Graph доступны в предварительной версии (в конечной точке `/beta`) во всех национальных облачных развертываниях, за исключением отмеченных.</span><span class="sxs-lookup"><span data-stu-id="e19a9-157">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e19a9-158">Контакты организации</span><span class="sxs-lookup"><span data-stu-id="e19a9-158">Organizational Contacts</span></span>
* <span data-ttu-id="e19a9-159">Приложения</span><span class="sxs-lookup"><span data-stu-id="e19a9-159">Applications</span></span>
* <span data-ttu-id="e19a9-160">Субъекты-службы</span><span class="sxs-lookup"><span data-stu-id="e19a9-160">Service Principals</span></span>

<span data-ttu-id="e19a9-161">Указанные ниже компоненты Microsoft Graph еще не поддерживаются в национальных облачных развертываниях:</span><span class="sxs-lookup"><span data-stu-id="e19a9-161">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="e19a9-162">Планировщик (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e19a9-162">Microsoft Planner</span></span>
* <span data-ttu-id="e19a9-163">Расширения схемы каталога</span><span class="sxs-lookup"><span data-stu-id="e19a9-163">Directory schema extensions</span></span>
* <span data-ttu-id="e19a9-164">Расширения открытого типа</span><span class="sxs-lookup"><span data-stu-id="e19a9-164">Open type extensions</span></span>
