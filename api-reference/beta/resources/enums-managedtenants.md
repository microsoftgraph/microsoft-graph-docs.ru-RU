---
title: Значения перечисления управления несколькими клиентами
description: Значения Graph управления несколькими клиентами
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: enumTypes
ms.openlocfilehash: 9b93794e763025b409ff00c0a2b5d13909ca705d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095953"
---
# <a name="multi-tenant-management-enumeration-values"></a>Значения перечисления управления несколькими клиентами

### <a name="delegatedprivilegestatus-values"></a>Значения delegatedPrivilegeStatus

|Member|
|:---|
|Нет|
|delegatedAdminPrivileges|
|unknownFutureValue|
|granularDelegatedAdminPrivileges|
|delegatedAndGranularDelegetedAdminPrivileges|

### <a name="managementactionstatus-values"></a>Значения managementActionStatus

|Member|
|:---|
|toAddress|
|Завершена|
|error|
|Времени ожидания|
|Inprogress|
|Планируется|
|resolvedBy3rdParty|
|resolvedThroughAlternateMitigation|
|riskAccepted|
|unknownFutureValue|

### <a name="managementcategory-values"></a>значения managementCategory

|Member|
|:---|
|Пользовательские|
|devices|
|Идентичности|
|unknownFutureValue|

### <a name="managementparametervaluetype-values"></a>Значения managementParameterValueType

|Member|
|:---|
|string|
|integer|
|логический|
|guid|
|Stringcollection|
|integerCollection|
|booleanCollection|
|guidCollection|
|unknownFutureValue|

### <a name="tenantonboardingstatus-values"></a>Значения tenantOnboardingStatus

|Member|
|:---|
|Недопустимые|
|inProcess|
|Активных|
|Неактивные|
|unknownFutureValue|

### <a name="tenantonboardingeligibilityreason-values"></a>Значения tenantOnboardingEligibilityReason

|Member|
|:---|
|Нет|
|contractType|
|delegatedAdminPrivileges|
|usersCount|
|license|
|unknownFutureValue|

### <a name="workloadactioncategory-values"></a>Значения workloadActionCategory

|Member|
|:---|
|Автоматизированные|
|Вручную|
|unknownFutureValue|

### <a name="workloadactionstatus-values"></a>Значения workloadActionStatus

|Member|
|:---|
|toAddress|
|Завершена|
|error|
|Времени ожидания|
|Inprogress|
|unknownFutureValue|

### <a name="workloadonboardingstatus-values"></a>Значения workloadOnboardingStatus

|Member|
|:---|
|notOnboarded|
|подключено|
|unknownFutureValue|
