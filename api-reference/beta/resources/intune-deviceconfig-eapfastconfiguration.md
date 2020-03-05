---
title: тип перечисления Еапфастконфигуратион
description: Доступные параметры настройки EAP – FAST.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: db3f39eaeb375705c974e907ae4b0a177bd6c4ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526548"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="588b8-103">тип перечисления Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="588b8-103">eapFastConfiguration enum type</span></span>

<span data-ttu-id="588b8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="588b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="588b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="588b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="588b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="588b8-107">Доступные параметры настройки EAP – FAST.</span><span class="sxs-lookup"><span data-stu-id="588b8-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="588b8-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="588b8-108">Members</span></span>
|<span data-ttu-id="588b8-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="588b8-109">Member</span></span>|<span data-ttu-id="588b8-110">Значение</span><span class="sxs-lookup"><span data-stu-id="588b8-110">Value</span></span>|<span data-ttu-id="588b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="588b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="588b8-112">нопротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="588b8-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="588b8-113">нуль</span><span class="sxs-lookup"><span data-stu-id="588b8-113">0</span></span>|<span data-ttu-id="588b8-114">Используйте EAP-FAST без безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="588b8-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="588b8-115">усепротектедакцесскредентиал</span><span class="sxs-lookup"><span data-stu-id="588b8-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="588b8-116">1 </span><span class="sxs-lookup"><span data-stu-id="588b8-116">1</span></span>|<span data-ttu-id="588b8-117">Использование учетных данных безопасного доступа (PAC).</span><span class="sxs-lookup"><span data-stu-id="588b8-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="588b8-118">усепротектедакцесскредентиаландпровисион</span><span class="sxs-lookup"><span data-stu-id="588b8-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="588b8-119">2 </span><span class="sxs-lookup"><span data-stu-id="588b8-119">2</span></span>|<span data-ttu-id="588b8-120">Использование учетных данных безопасного доступа (PAC) и подготовка ключа PAC.</span><span class="sxs-lookup"><span data-stu-id="588b8-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="588b8-121">усепротектедакцесскредентиаландпровисионанонимаусли</span><span class="sxs-lookup"><span data-stu-id="588b8-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="588b8-122">3 </span><span class="sxs-lookup"><span data-stu-id="588b8-122">3</span></span>|<span data-ttu-id="588b8-123">Использование учетных данных безопасного доступа (PAC), подготовка ключа PAC и анонимное выполнение.</span><span class="sxs-lookup"><span data-stu-id="588b8-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|



