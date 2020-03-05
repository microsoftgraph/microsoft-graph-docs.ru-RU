---
title: Общие сведения об API политики
description: Azure Active Directory использует политики для управления поведением компонентов Azure AD в вашей организации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c439cf8f53a6ce7a9be146e02888ba4a819101ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521616"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="59486-103">Общие сведения о политике Azure AD</span><span class="sxs-lookup"><span data-stu-id="59486-103">Azure AD policy overview</span></span>

<span data-ttu-id="59486-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59486-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59486-105">Azure Active Directory (Azure AD) использует политики для управления поведением компонентов Azure AD в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="59486-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="59486-106">Политики это настраиваемые правила, которые можно применять к приложениям, субъектам, группам или всем организациям, которым они назначены.</span><span class="sxs-lookup"><span data-stu-id="59486-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="59486-107">Какие политики доступны?</span><span class="sxs-lookup"><span data-stu-id="59486-107">What policies are available?</span></span>

| <span data-ttu-id="59486-108">Тип политики</span><span class="sxs-lookup"><span data-stu-id="59486-108">Policy type</span></span>       | <span data-ttu-id="59486-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59486-109">Description</span></span> | <span data-ttu-id="59486-110">Примеры</span><span class="sxs-lookup"><span data-stu-id="59486-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="59486-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="59486-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="59486-112">Представляет политику, которая управляет автоматическим выходом для веб-сеансов после определенного периода бездействия для приложений, поддерживающих функции времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="59486-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="59486-113">Настройте на портале Azure время ожидания простоя в 15 минут.</span><span class="sxs-lookup"><span data-stu-id="59486-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="59486-114">claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="59486-114">claimsMappingPolicies</span></span>](claimsMappingPolicy.md)| <span data-ttu-id="59486-115">Представляет политики сопоставления утверждений для протоколов WS — подача, SAML, OAuth 2,0 и OpenID Connect для маркеров, выданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="59486-115">Represents the claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.</span></span> | <span data-ttu-id="59486-116">Создайте и назначьте политику для пропуска базовых утверждений от маркеров, выданных участнику службы.</span><span class="sxs-lookup"><span data-stu-id="59486-116">Create and assign a policy to omit the basic claims from tokens issued to a service principal.</span></span> |
|[<span data-ttu-id="59486-117">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="59486-117">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="59486-118">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="59486-118">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="59486-119">Настройте все пользователи для пропуска обнаружения домашней области и маршрутизации непосредственно в ADFS для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="59486-119">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="59486-120">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="59486-120">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="59486-121">Представляет срок жизни маркеров доступа, используемых для доступа к защищенным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="59486-121">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="59486-122">Настройка особенно конфиденциального приложения с использованием более короткого срока действия маркера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="59486-122">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="59486-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="59486-123">Next steps</span></span>

* <span data-ttu-id="59486-124">Просмотрите различные типы ресурсов политики, перечисленные выше, и их различные методы.</span><span class="sxs-lookup"><span data-stu-id="59486-124">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="59486-125">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="59486-125">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
