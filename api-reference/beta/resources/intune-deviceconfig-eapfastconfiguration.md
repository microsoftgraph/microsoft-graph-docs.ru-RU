---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7acf6ffbf7a93bc5002f7f81679fc789ab313e2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567146"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="edea6-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="edea6-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="edea6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edea6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edea6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edea6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edea6-106">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="edea6-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="edea6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="edea6-107">Members</span></span>
|<span data-ttu-id="edea6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="edea6-108">Member</span></span>|<span data-ttu-id="edea6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="edea6-109">Value</span></span>|<span data-ttu-id="edea6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="edea6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edea6-111">Нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="edea6-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="edea6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="edea6-112">0</span></span>|<span data-ttu-id="edea6-113">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="edea6-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="edea6-114">Усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="edea6-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="edea6-115">1 </span><span class="sxs-lookup"><span data-stu-id="edea6-115">1</span></span>|<span data-ttu-id="edea6-116">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="edea6-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="edea6-117">Усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="edea6-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="edea6-118">2 </span><span class="sxs-lookup"><span data-stu-id="edea6-118">2</span></span>|<span data-ttu-id="edea6-119">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="edea6-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="edea6-120">Усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="edea6-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="edea6-121">3 </span><span class="sxs-lookup"><span data-stu-id="edea6-121">3</span></span>|<span data-ttu-id="edea6-122">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="edea6-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





