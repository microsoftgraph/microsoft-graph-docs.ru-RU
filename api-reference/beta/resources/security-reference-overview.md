---
title: Использование API Microsoft Graph для обнаружения и защиты угроз безопасности (Предварительная версия)
description: Более изощренные угрозы безопасности продолжают расширять, что влияет на глобальную экономию. В организациях часто приходится нанести ущерб, пока Организация даже обнаружит ее. С помощью Microsoft Graph можно создавать или расширять решения для обеспечения безопасности, объединяющие и соотнесение оповещений системы безопасности из нескольких источников, обнаруживать угрозы, которые пытаются подвергнуться нарушению удостоверения пользователя, разблокировать контекстные данные для информирования об расследовании и автоматизировать операции безопасности для повышения эффективности.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 5550509e3ececdb159125e66c1bd12962722832d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988900"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="29bf2-105">Использование API Microsoft Graph для обнаружения и защиты угроз безопасности (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="29bf2-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

<span data-ttu-id="29bf2-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29bf2-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29bf2-107">Более изощренные угрозы безопасности продолжают расширять, что влияет на глобальную экономию.</span><span class="sxs-lookup"><span data-stu-id="29bf2-107">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="29bf2-108">В организациях часто приходится нанести ущерб, пока Организация даже обнаружит ее.</span><span class="sxs-lookup"><span data-stu-id="29bf2-108">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="29bf2-109">С помощью Microsoft Graph можно создавать или расширять решения для обеспечения безопасности, объединяющие и соотнесение оповещений системы безопасности из нескольких источников, обнаруживать угрозы, которые пытаются подвергнуться нарушению удостоверения пользователя, разблокировать контекстные данные для информирования об расследовании и автоматизировать операции безопасности для повышения эффективности.</span><span class="sxs-lookup"><span data-stu-id="29bf2-109">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="29bf2-110">Интеллектуальный граф безопасности объединяет логику безопасности в центрах безопасности Майкрософт, центрах безопасности и партнерах из всего мира, образуя экосистему интегрированных решений безопасности.</span><span class="sxs-lookup"><span data-stu-id="29bf2-110">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="29bf2-111">С помощью машинного обучения, мониторинга поведений и масштаба облака интеллектуальный граф безопасности позволяет быстрее и эффективно защищать, обнаруживать и отвечать на угрозы.</span><span class="sxs-lookup"><span data-stu-id="29bf2-111">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="29bf2-112">[API безопасности](security-api-overview.md) подключается к [интеллектуальному графу безопасности](https://www.microsoft.com/en-us/security/intelligence-security-api)и предоставляет решения, которые являются действиями и целостностью.</span><span class="sxs-lookup"><span data-stu-id="29bf2-112">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="29bf2-113">[API рисков для защиты удостоверений](identityprotection-root.md) предоставляет легкий доступ для пользователей Azure AD Premium P1 и P2 для отправки запросов на [обнаружение рисков, выполняемых защитой удостоверений](/azure/active-directory/active-directory-identityprotection-graph-getting-started) , и использовать эти события в системах SIEM и приложениях безопасности.</span><span class="sxs-lookup"><span data-stu-id="29bf2-113">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="29bf2-114">См. также</span><span class="sxs-lookup"><span data-stu-id="29bf2-114">See also</span></span>

- [<span data-ttu-id="29bf2-115">Зачем использовать API безопасности?</span><span class="sxs-lookup"><span data-stu-id="29bf2-115">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="29bf2-116">Интеграция с интеллектуальным графиком безопасности с помощью API безопасности</span><span class="sxs-lookup"><span data-stu-id="29bf2-116">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- [<span data-ttu-id="29bf2-117">Зачем использовать Azure AD для защиты удостоверений в вашей организации?</span><span class="sxs-lookup"><span data-stu-id="29bf2-117">Why use Azure AD to protect identities in your organization?</span></span>](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)
- [<span data-ttu-id="29bf2-118">Использование API защиты удостоверений Azure AD</span><span class="sxs-lookup"><span data-stu-id="29bf2-118">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)


