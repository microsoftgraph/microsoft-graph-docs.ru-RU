---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0d8a250b2272ae8b8287f9869697633493b116f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173572"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="5697c-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5697c-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="5697c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5697c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5697c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5697c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5697c-106">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="5697c-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="5697c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="5697c-107">Members</span></span>
|<span data-ttu-id="5697c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="5697c-108">Member</span></span>|<span data-ttu-id="5697c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="5697c-109">Value</span></span>|<span data-ttu-id="5697c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5697c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5697c-111">Нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="5697c-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="5697c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="5697c-112">0</span></span>|<span data-ttu-id="5697c-113">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="5697c-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="5697c-114">Усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="5697c-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="5697c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="5697c-115">1</span></span>|<span data-ttu-id="5697c-116">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="5697c-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="5697c-117">Усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="5697c-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="5697c-118">2</span><span class="sxs-lookup"><span data-stu-id="5697c-118">2</span></span>|<span data-ttu-id="5697c-119">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="5697c-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="5697c-120">Усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="5697c-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="5697c-121">4</span><span class="sxs-lookup"><span data-stu-id="5697c-121">3</span></span>|<span data-ttu-id="5697c-122">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="5697c-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




