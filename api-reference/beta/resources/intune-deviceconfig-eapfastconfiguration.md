---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fada1b937e8a4d946a5ef12687692f59ae90b383
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003747"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="027ef-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="027ef-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="027ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="027ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="027ef-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="027ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="027ef-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="027ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="027ef-107">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="027ef-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="027ef-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="027ef-108">Members</span></span>
|<span data-ttu-id="027ef-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="027ef-109">Member</span></span>|<span data-ttu-id="027ef-110">Значение</span><span class="sxs-lookup"><span data-stu-id="027ef-110">Value</span></span>|<span data-ttu-id="027ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="027ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="027ef-112">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="027ef-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="027ef-113">нуль</span><span class="sxs-lookup"><span data-stu-id="027ef-113">0</span></span>|<span data-ttu-id="027ef-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="027ef-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="027ef-115">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="027ef-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="027ef-116">1 </span><span class="sxs-lookup"><span data-stu-id="027ef-116">1</span></span>|<span data-ttu-id="027ef-117">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="027ef-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="027ef-118">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="027ef-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="027ef-119">2 </span><span class="sxs-lookup"><span data-stu-id="027ef-119">2</span></span>|<span data-ttu-id="027ef-120">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="027ef-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="027ef-121">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="027ef-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="027ef-122">4</span><span class="sxs-lookup"><span data-stu-id="027ef-122">3</span></span>|<span data-ttu-id="027ef-123">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="027ef-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|






