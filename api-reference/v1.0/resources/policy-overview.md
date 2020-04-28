---
title: Общие сведения об API политики
description: Azure Active Directory использует политики для управления поведением компонентов Azure AD в вашей организации.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c34d8114e90aaf3c680ed89da4d16cd12880e71e
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917553"
---
# <a name="azure-ad-policy-overview"></a><span data-ttu-id="08522-103">Общие сведения о политике Azure AD</span><span class="sxs-lookup"><span data-stu-id="08522-103">Azure AD policy overview</span></span>

<span data-ttu-id="08522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08522-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="08522-105">Azure Active Directory (Azure AD) использует политики для управления поведением компонентов Azure AD в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="08522-105">Azure Active Directory (Azure AD) uses policies to control Azure AD feature behaviors in your organization.</span></span> <span data-ttu-id="08522-106">Политики это настраиваемые правила, которые можно применять к приложениям, субъектам, группам или всем организациям, которым они назначены.</span><span class="sxs-lookup"><span data-stu-id="08522-106">Policies are custom rules that you can enforce on applications, service principals, groups, or on the entire organization they are assigned to.</span></span>

## <a name="what-policies-are-available"></a><span data-ttu-id="08522-107">Какие политики доступны?</span><span class="sxs-lookup"><span data-stu-id="08522-107">What policies are available?</span></span>

| <span data-ttu-id="08522-108">Тип политики</span><span class="sxs-lookup"><span data-stu-id="08522-108">Policy type</span></span>       | <span data-ttu-id="08522-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08522-109">Description</span></span> | <span data-ttu-id="08522-110">Примеры</span><span class="sxs-lookup"><span data-stu-id="08522-110">Examples</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="08522-111">activityBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="08522-111">activityBasedTimeoutPolicies</span></span>](activityBasedTimeoutPolicy.md)| <span data-ttu-id="08522-112">Представляет политику, которая управляет автоматическим выходом для веб-сеансов после определенного периода бездействия для приложений, поддерживающих функции времени ожидания на основе действий.</span><span class="sxs-lookup"><span data-stu-id="08522-112">Represents a policy that controls automatic sign-out for web sessions after a period of inactivity, for applications that support activity-based timeout functionality.</span></span>| <span data-ttu-id="08522-113">Настройте на портале Azure время ожидания простоя в 15 минут.</span><span class="sxs-lookup"><span data-stu-id="08522-113">Configure the Azure portal to have an inactivity timeout of 15 minutes.</span></span> |
|[<span data-ttu-id="08522-114">homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="08522-114">homeRealmDiscoveryPolicies</span></span>](homeRealmDiscoveryPolicy.md)| <span data-ttu-id="08522-115">Представляет политику для управления поведением проверки подлинности Azure Active Directory для федеративных пользователей, в частности для ограничений автоматического ускорения и проверки подлинности пользователей в федеративных доменах.</span><span class="sxs-lookup"><span data-stu-id="08522-115">Represents a policy to control Azure Active Directory authentication behavior for federated users, in particular for auto-acceleration and user authentication restrictions in federated domains.</span></span>| <span data-ttu-id="08522-116">Настройте все пользователи для пропуска обнаружения домашней области и маршрутизации непосредственно в ADFS для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="08522-116">Configure all users to skip home realm discovery and be routed directly to ADFS for authentication.</span></span> |
|[<span data-ttu-id="08522-117">tokenLifetimePolicies</span><span class="sxs-lookup"><span data-stu-id="08522-117">tokenLifetimePolicies</span></span>](tokenlifetimepolicy.md)|<span data-ttu-id="08522-118">Представляет срок жизни маркеров доступа, используемых для доступа к защищенным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="08522-118">Represents the lifetime duration of access tokens used to access protected resources.</span></span>| <span data-ttu-id="08522-119">Настройка особенно конфиденциального приложения с использованием более короткого срока действия маркера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="08522-119">Configure a particularly sensitive application with a shorter than default token lifetime.</span></span>|
|[<span data-ttu-id="08522-120">токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="08522-120">tokenIssuancePolicy</span></span>](tokenIssuancePolicy.md)|<span data-ttu-id="08522-121">Представляет политику, определяющую характеристики маркеров SAML, выданных Azure AD.</span><span class="sxs-lookup"><span data-stu-id="08522-121">Represents the policy to specify the characteristics of SAML tokens issued by Azure AD.</span></span>| <span data-ttu-id="08522-122">Настройте алгоритм подписи или версию токена SAML, которые будут использоваться для выдачи маркера SAML.</span><span class="sxs-lookup"><span data-stu-id="08522-122">Configure the signing algorithm or SAML token version to be used to issue the SAML token.</span></span>

## <a name="next-steps"></a><span data-ttu-id="08522-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="08522-123">Next steps</span></span>

* <span data-ttu-id="08522-124">Просмотрите различные типы ресурсов политики, перечисленные выше, и их различные методы.</span><span class="sxs-lookup"><span data-stu-id="08522-124">Review the different policy resouce types listed above and their various methods.</span></span>
* <span data-ttu-id="08522-125">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="08522-125">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
