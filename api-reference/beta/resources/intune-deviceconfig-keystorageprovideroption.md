---
title: тип перечисления Кэйсторажепровидероптион
description: Параметры импорта поставщика хранилища ключей (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460424"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="eabc9-103">тип перечисления Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="eabc9-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="eabc9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eabc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eabc9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eabc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eabc9-106">Параметры импорта поставщика хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="eabc9-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="eabc9-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="eabc9-107">Members</span></span>
|<span data-ttu-id="eabc9-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="eabc9-108">Member</span></span>|<span data-ttu-id="eabc9-109">Значение</span><span class="sxs-lookup"><span data-stu-id="eabc9-109">Value</span></span>|<span data-ttu-id="eabc9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eabc9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eabc9-111">Усетпмкспосервисеусесофтварексп</span><span class="sxs-lookup"><span data-stu-id="eabc9-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="eabc9-112">нуль</span><span class="sxs-lookup"><span data-stu-id="eabc9-112">0</span></span>|<span data-ttu-id="eabc9-113">Импорт в KSP доверенного платформенного модуля (TPM), если он присутствует, в противном случае импортировать в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="eabc9-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="eabc9-114">Усетпмкспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="eabc9-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="eabc9-115">1,1</span><span class="sxs-lookup"><span data-stu-id="eabc9-115">1</span></span>|<span data-ttu-id="eabc9-116">Импорт в KSP доверенного ПЛАТФОРМЕНного модуля (TPM), если он присутствует, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="eabc9-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="eabc9-117">Усепасспортфорворккспосервисефаил</span><span class="sxs-lookup"><span data-stu-id="eabc9-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="eabc9-118">2</span><span class="sxs-lookup"><span data-stu-id="eabc9-118">2</span></span>|<span data-ttu-id="eabc9-119">Импорт в паспорт для Works KSP, если он доступен, в противном случае произойдет ошибка.</span><span class="sxs-lookup"><span data-stu-id="eabc9-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="eabc9-120">Усесофтварексп</span><span class="sxs-lookup"><span data-stu-id="eabc9-120">useSoftwareKsp</span></span>|<span data-ttu-id="eabc9-121">4</span><span class="sxs-lookup"><span data-stu-id="eabc9-121">3</span></span>|<span data-ttu-id="eabc9-122">Импорт в KSP программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="eabc9-122">Import to Software KSP.</span></span>|





