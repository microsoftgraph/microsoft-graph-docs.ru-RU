---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399390"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="fa846-103">Тип перечисления eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa846-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="fa846-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa846-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa846-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa846-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa846-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa846-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa846-107">Доступные параметры для конфигурации EAP-FAST.</span><span class="sxs-lookup"><span data-stu-id="fa846-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="fa846-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fa846-108">Members</span></span>
|<span data-ttu-id="fa846-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fa846-109">Member</span></span>|<span data-ttu-id="fa846-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fa846-110">Value</span></span>|<span data-ttu-id="fa846-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa846-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa846-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="fa846-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="fa846-113">0</span><span class="sxs-lookup"><span data-stu-id="fa846-113">0</span></span>|<span data-ttu-id="fa846-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="fa846-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="fa846-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="fa846-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="fa846-116">1</span><span class="sxs-lookup"><span data-stu-id="fa846-116">1</span></span>|<span data-ttu-id="fa846-117">Использование защиты безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="fa846-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="fa846-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="fa846-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="fa846-119">2</span><span class="sxs-lookup"><span data-stu-id="fa846-119">2</span></span>|<span data-ttu-id="fa846-120">Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные</span><span class="sxs-lookup"><span data-stu-id="fa846-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="fa846-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="fa846-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="fa846-122">3</span><span class="sxs-lookup"><span data-stu-id="fa846-122">3</span></span>|<span data-ttu-id="fa846-123">Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.</span><span class="sxs-lookup"><span data-stu-id="fa846-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




