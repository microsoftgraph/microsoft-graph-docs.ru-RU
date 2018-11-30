---
title: Тип перечисления secureAssessmentAccountType
description: Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.
ms.openlocfilehash: 97dc60d8d15e90c43923d939cf957e1092b2cc45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080883"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="7b8bf-103">Тип перечисления secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="7b8bf-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="7b8bf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b8bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b8bf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b8bf-107">Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="7b8bf-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="7b8bf-108">Members</span></span>
|<span data-ttu-id="7b8bf-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="7b8bf-109">Member</span></span>|<span data-ttu-id="7b8bf-110">Значение</span><span class="sxs-lookup"><span data-stu-id="7b8bf-110">Value</span></span>|<span data-ttu-id="7b8bf-111">Description</span><span class="sxs-lookup"><span data-stu-id="7b8bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b8bf-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="7b8bf-112">azureADAccount</span></span>|<span data-ttu-id="7b8bf-113">0</span><span class="sxs-lookup"><span data-stu-id="7b8bf-113">0</span></span>|<span data-ttu-id="7b8bf-114">Указывает учетную запись Azure AD в формате AzureAD\ username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="7b8bf-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="7b8bf-115">domainAccount</span></span>|<span data-ttu-id="7b8bf-116">1</span><span class="sxs-lookup"><span data-stu-id="7b8bf-116">1</span></span>|<span data-ttu-id="7b8bf-117">Указывает учетную запись домена в формате "домен\пользователь" или user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="7b8bf-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="7b8bf-118">localAccount</span></span>|<span data-ttu-id="7b8bf-119">2</span><span class="sxs-lookup"><span data-stu-id="7b8bf-119">2</span></span>|<span data-ttu-id="7b8bf-120">Указывает локальной учетной записи в формате имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b8bf-120">Indicates a local account in format of username.</span></span>|





