---
title: Использование Microsoft Graph API для обнаружения угроз безопасности и защиты (Предварительная версия)
description: Сложность угрозы безопасности по-прежнему производится перевод, влияния на глобальной экономики. Повреждение чаще всего осуществляется за срок перед организациями даже обнаружения его. Microsoft Graph можно использовать для построения или расширить, объединение и соотнесения оповещение системы безопасности из нескольких источников, обнаружения угроз, которые пытаются злоумышленнику удостоверения пользователя, unlock контекстных данных для автоматизации и информирование расследований решения по обеспечению безопасности операции по безопасности для повышения эффективности.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 37e98203e8f031aa98b35d82110a69e434c22a3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529931"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="849ec-105">Использование Microsoft Graph API для обнаружения угроз безопасности и защиты (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="849ec-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="849ec-106">Сложность угрозы безопасности по-прежнему производится перевод, влияния на глобальной экономики.</span><span class="sxs-lookup"><span data-stu-id="849ec-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="849ec-107">Повреждение чаще всего осуществляется за срок перед организациями даже обнаружения его.</span><span class="sxs-lookup"><span data-stu-id="849ec-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="849ec-108">Microsoft Graph можно использовать для построения или расширить, объединение и соотнесения оповещение системы безопасности из нескольких источников, обнаружения угроз, которые пытаются злоумышленнику удостоверения пользователя, unlock контекстных данных для автоматизации и информирование расследований решения по обеспечению безопасности операции по безопасности для повышения эффективности.</span><span class="sxs-lookup"><span data-stu-id="849ec-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="849ec-109">Интеллектуальный график безопасности объединяет аналитики безопасности из в рамках Microsoft, центры операций по безопасности и партнеры из по всему миру для формирования экосистемы решений интегрированная система безопасности.</span><span class="sxs-lookup"><span data-stu-id="849ec-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="849ec-110">С помощью машинного обучения, поведения мониторинга и масштаба облаке, Intelligent график безопасности можно лучше защитить, обнаружение и реагировать на угрозы, связанные с быстро и комплексно.</span><span class="sxs-lookup"><span data-stu-id="849ec-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="849ec-111">[Безопасность API](security-api-overview.md) для подключения к на [Графике Intelligent безопасности](https://www.microsoft.com/en-us/security/intelligence-security-api), повышая вы работы с решениями, предусматривающей действие и комплексный.</span><span class="sxs-lookup"><span data-stu-id="849ec-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="849ec-112">[События рисков защиты удостоверения API](identityprotection-root.md) предоставляет легкий доступ для Azure AD Premium P1 и P2 клиентов для запроса [обнаружения риск, сделанных с идентификатором защиты](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) и использовать эти события в SIEM систем и безопасность приложений.</span><span class="sxs-lookup"><span data-stu-id="849ec-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="849ec-113">См. также</span><span class="sxs-lookup"><span data-stu-id="849ec-113">See also</span></span>

- [<span data-ttu-id="849ec-114">Причины использования безопасности API?</span><span class="sxs-lookup"><span data-stu-id="849ec-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="849ec-115">Использование безопасности API для интеграции с Intelligent график безопасности</span><span class="sxs-lookup"><span data-stu-id="849ec-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- <span data-ttu-id="849ec-116">Зачем использовать Azure AD для защиты удостоверений в организации?</span><span class="sxs-lookup"><span data-stu-id="849ec-116">[Why use Azure AD to protect identities in your organization?](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)</span></span>
- [<span data-ttu-id="849ec-117">Использование API защиты идентификации Azure AD</span><span class="sxs-lookup"><span data-stu-id="849ec-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-reference-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
