---
title: Тип перечисления zebraFotaDeploymentState
description: Представляет состояние развертывания Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5912f89249951db9ff4dd5a058169cb3b54113fc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213567"
---
# <a name="zebrafotadeploymentstate-enum-type"></a>Тип перечисления zebraFotaDeploymentState

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет состояние развертывания Zebra FOTA.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|pendingCreation|0|Развертывание создано, но Zebra не подтверждает его создание.|
|createFailed|1|Развертывание не было успешно создано с помощью Zebra.|
|создано|2|Развертывание создано, но еще не развернуто.|
|Inprogress|3|Развертывание запущено, но не завершено.|
|Завершена|4|Развертывание завершено или дата окончания завершена.|
|pendingCancel|5|Администратор запросит отмену развертывания, но Zebra не подтверждает отмену.|
|Отменен|6 |Zebra успешно отменил развертывание.|
|unknownFutureValue|99|Неизвестное значение перечисления в будущем.|




