---
title: Тип перечисления secureAssessmentAccountType
description: Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b1f8a3d03c0e7b9e91c68ff5a87611fcaa6f31e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826056"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="fe416-103">Тип перечисления secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="fe416-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="fe416-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe416-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe416-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe416-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe416-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe416-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe416-107">Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="fe416-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="fe416-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fe416-108">Members</span></span>
|<span data-ttu-id="fe416-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fe416-109">Member</span></span>|<span data-ttu-id="fe416-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fe416-110">Value</span></span>|<span data-ttu-id="fe416-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe416-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe416-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="fe416-112">azureADAccount</span></span>|<span data-ttu-id="fe416-113">0</span><span class="sxs-lookup"><span data-stu-id="fe416-113">0</span></span>|<span data-ttu-id="fe416-114">Указывает учетную запись Azure AD в формате AzureAD\ username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="fe416-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="fe416-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="fe416-115">domainAccount</span></span>|<span data-ttu-id="fe416-116">1</span><span class="sxs-lookup"><span data-stu-id="fe416-116">1</span></span>|<span data-ttu-id="fe416-117">Указывает учетную запись домена в формате "домен\пользователь" или user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="fe416-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="fe416-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="fe416-118">localAccount</span></span>|<span data-ttu-id="fe416-119">2</span><span class="sxs-lookup"><span data-stu-id="fe416-119">2</span></span>|<span data-ttu-id="fe416-120">Указывает локальной учетной записи в формате имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="fe416-120">Indicates a local account in format of username.</span></span>|





