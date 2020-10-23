---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15232635cfcbe5064c5efe7beeb05e58c5e321ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701552"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="60cd7-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="60cd7-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="60cd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60cd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60cd7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60cd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60cd7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60cd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60cd7-107">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="60cd7-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="60cd7-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="60cd7-108">Members</span></span>
|<span data-ttu-id="60cd7-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="60cd7-109">Member</span></span>|<span data-ttu-id="60cd7-110">Значение</span><span class="sxs-lookup"><span data-stu-id="60cd7-110">Value</span></span>|<span data-ttu-id="60cd7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60cd7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60cd7-112">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="60cd7-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="60cd7-113">нуль</span><span class="sxs-lookup"><span data-stu-id="60cd7-113">0</span></span>|<span data-ttu-id="60cd7-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="60cd7-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="60cd7-115">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="60cd7-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="60cd7-116">1,1</span><span class="sxs-lookup"><span data-stu-id="60cd7-116">1</span></span>|<span data-ttu-id="60cd7-117">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="60cd7-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="60cd7-118">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="60cd7-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="60cd7-119">2</span><span class="sxs-lookup"><span data-stu-id="60cd7-119">2</span></span>|<span data-ttu-id="60cd7-120">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="60cd7-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="60cd7-121">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="60cd7-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="60cd7-122">4</span><span class="sxs-lookup"><span data-stu-id="60cd7-122">3</span></span>|<span data-ttu-id="60cd7-123">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="60cd7-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





