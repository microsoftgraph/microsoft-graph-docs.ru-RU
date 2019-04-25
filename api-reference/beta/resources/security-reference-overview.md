---
title: Использование API Microsoft Graph для обнаружения и защиты угроз безопасности (Предварительная версия)
description: Более изощренные угрозы безопасности продолжают расширять, что влияет на глобальную экономию. В организациях часто приходится наНести ущерб, пока Организация даже обнаружит ее. С помощью Microsoft Graph можно создавать или расширять решения для обеспечения безопасности, объединяющие и соотнесение оповещений системы безопасности из нескольких источников, обнаруживать угрозы, которые пытаются нарушить безопасность удостоверения пользователя, разблокировать контекстные данные для информирования об расследованиях и автоматизации повышение эффективности операций безопасности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 37e98203e8f031aa98b35d82110a69e434c22a3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524465"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="76c49-105">Использование API Microsoft Graph для обнаружения и защиты угроз безопасности (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="76c49-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c49-106">Более изощренные угрозы безопасности продолжают расширять, что влияет на глобальную экономию.</span><span class="sxs-lookup"><span data-stu-id="76c49-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="76c49-107">В организациях часто приходится наНести ущерб, пока Организация даже обнаружит ее.</span><span class="sxs-lookup"><span data-stu-id="76c49-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="76c49-108">С помощью Microsoft Graph можно создавать или расширять решения для обеспечения безопасности, объединяющие и соотнесение оповещений системы безопасности из нескольких источников, обнаруживать угрозы, которые пытаются нарушить безопасность удостоверения пользователя, разблокировать контекстные данные для информирования об расследованиях и автоматизации повышение эффективности операций безопасности.</span><span class="sxs-lookup"><span data-stu-id="76c49-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="76c49-109">Интеллектуальный граф безопасности объединяет логику безопасности в центрах безопасности Майкрософт, центрах безопасности и партнерах из всего мира, образуя экосистему интегрированных решений безопасности.</span><span class="sxs-lookup"><span data-stu-id="76c49-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="76c49-110">С помощью машинного обучения, мониторинга поведений и масштаба облака интеллектуальный граф безопасности позволяет быстрее и эффективно защищать, обнаруживать и отвечать на угрозы.</span><span class="sxs-lookup"><span data-stu-id="76c49-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="76c49-111">[API безопасности](security-api-overview.md) подключается к [интеллектуальнОму графу безопасности](https://www.microsoft.com/en-us/security/intelligence-security-api)и предоставляет решения, которые являются действиями и целостностью.</span><span class="sxs-lookup"><span data-stu-id="76c49-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="76c49-112">[API рисков для защиты удостоверений](identityprotection-root.md) предоставляет легкий доступ для пользователей Azure AD Premium P1 и P2 для отправки запросов на [обнаружение рисков, выполняемЫх защитой удостоверений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) , и использовать эти события в системах SIEM и приложениях безопасности.</span><span class="sxs-lookup"><span data-stu-id="76c49-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="76c49-113">См. также</span><span class="sxs-lookup"><span data-stu-id="76c49-113">See also</span></span>

- [<span data-ttu-id="76c49-114">Зачем использовать API безопасности?</span><span class="sxs-lookup"><span data-stu-id="76c49-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="76c49-115">Интеграция с интеллектуальным графиком безопасности с помощью API безопасности</span><span class="sxs-lookup"><span data-stu-id="76c49-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- [<span data-ttu-id="76c49-116">Зачем использовать Azure AD для защиты удостоверений в вашей организации?</span><span class="sxs-lookup"><span data-stu-id="76c49-116">Why use Azure AD to protect identities in your organization?</span></span>](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)
- [<span data-ttu-id="76c49-117">Использование API защиты удостоверений Azure AD</span><span class="sxs-lookup"><span data-stu-id="76c49-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-reference-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
