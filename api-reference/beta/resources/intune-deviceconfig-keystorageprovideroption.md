---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a2612aeb2cded950023a14136b71a8c7a55555a9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790414"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="59d17-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="59d17-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="59d17-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59d17-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59d17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59d17-106">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="59d17-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="59d17-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="59d17-107">Members</span></span>
|<span data-ttu-id="59d17-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="59d17-108">Member</span></span>|<span data-ttu-id="59d17-109">Значение</span><span class="sxs-lookup"><span data-stu-id="59d17-109">Value</span></span>|<span data-ttu-id="59d17-110">Описание</span><span class="sxs-lookup"><span data-stu-id="59d17-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d17-111">усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="59d17-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="59d17-112">нуль</span><span class="sxs-lookup"><span data-stu-id="59d17-112">0</span></span>|<span data-ttu-id="59d17-113">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="59d17-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="59d17-114">усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="59d17-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="59d17-115">1,1</span><span class="sxs-lookup"><span data-stu-id="59d17-115">1</span></span>|<span data-ttu-id="59d17-116">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="59d17-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="59d17-117">усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="59d17-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="59d17-118">2</span><span class="sxs-lookup"><span data-stu-id="59d17-118">2</span></span>|<span data-ttu-id="59d17-119">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="59d17-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="59d17-120">усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="59d17-120">useSoftwareKsp</span></span>|<span data-ttu-id="59d17-121">4</span><span class="sxs-lookup"><span data-stu-id="59d17-121">3</span></span>|<span data-ttu-id="59d17-122">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="59d17-122">Import to Software KSP.</span></span>|



