---
title: Тип перечисления secureAssessmentAccountType
description: Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e5ae78b5df3636e738cf21beece269e6fa7b81a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959260"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="e802d-103">Тип перечисления secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="e802d-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="e802d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e802d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e802d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e802d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e802d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e802d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e802d-107">Тип учетных записей, которые разрешены для Windows10SecureAssessment ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="e802d-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="e802d-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e802d-108">Members</span></span>
|<span data-ttu-id="e802d-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e802d-109">Member</span></span>|<span data-ttu-id="e802d-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e802d-110">Value</span></span>|<span data-ttu-id="e802d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e802d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e802d-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="e802d-112">azureADAccount</span></span>|<span data-ttu-id="e802d-113">0</span><span class="sxs-lookup"><span data-stu-id="e802d-113">0</span></span>|<span data-ttu-id="e802d-114">Указывает учетную запись Azure AD в формате AzureAD\ username@tenant.com.</span><span class="sxs-lookup"><span data-stu-id="e802d-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="e802d-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="e802d-115">domainAccount</span></span>|<span data-ttu-id="e802d-116">1</span><span class="sxs-lookup"><span data-stu-id="e802d-116">1</span></span>|<span data-ttu-id="e802d-117">Указывает учетную запись домена в формате "домен\пользователь" или user@domain.com.</span><span class="sxs-lookup"><span data-stu-id="e802d-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="e802d-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="e802d-118">localAccount</span></span>|<span data-ttu-id="e802d-119">2</span><span class="sxs-lookup"><span data-stu-id="e802d-119">2</span></span>|<span data-ttu-id="e802d-120">Указывает локальной учетной записи в формате имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e802d-120">Indicates a local account in format of username.</span></span>|





