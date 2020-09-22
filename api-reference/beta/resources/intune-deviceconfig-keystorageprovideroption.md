---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4013afe6f39decefec32cc3fe68f3236b43ee60f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092498"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="4dcf5-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="4dcf5-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="4dcf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dcf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dcf5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dcf5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dcf5-107">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="4dcf5-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="4dcf5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="4dcf5-108">Members</span></span>
|<span data-ttu-id="4dcf5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="4dcf5-109">Member</span></span>|<span data-ttu-id="4dcf5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4dcf5-110">Value</span></span>|<span data-ttu-id="4dcf5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4dcf5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dcf5-112">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="4dcf5-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="4dcf5-113">нуль</span><span class="sxs-lookup"><span data-stu-id="4dcf5-113">0</span></span>|<span data-ttu-id="4dcf5-114">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="4dcf5-115">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="4dcf5-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="4dcf5-116">1 </span><span class="sxs-lookup"><span data-stu-id="4dcf5-116">1</span></span>|<span data-ttu-id="4dcf5-117">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="4dcf5-118">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="4dcf5-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="4dcf5-119">2 </span><span class="sxs-lookup"><span data-stu-id="4dcf5-119">2</span></span>|<span data-ttu-id="4dcf5-120">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="4dcf5-121">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="4dcf5-121">useSoftwareKsp</span></span>|<span data-ttu-id="4dcf5-122">4</span><span class="sxs-lookup"><span data-stu-id="4dcf5-122">3</span></span>|<span data-ttu-id="4dcf5-123">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="4dcf5-123">Import to Software KSP.</span></span>|






