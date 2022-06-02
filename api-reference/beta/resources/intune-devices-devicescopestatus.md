---
title: Тип перечисления deviceScopeStatus
description: 'Указывает состояние области устройства после включения области устройства. Возможные значения: none, computing, insufficientData или completed. Значение по умолчанию — none.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8347440c0c02f0f6c148717457616a19c22bc03f
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858832"
---
# <a name="devicescopestatus-enum-type"></a>Тип перечисления deviceScopeStatus

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает состояние области устройства после включения области устройства. Возможные значения: none, computing, insufficientData или completed. Значение по умолчанию — none.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Указывает, что область устройства не включена и вычисления не выполняются.|
|Вычислений|1|Указывает, что область устройства включена и данные метрик отчета пересчитываются службой.|
|insufficientData|2|Указывает, что область устройства включена, но недостаточно данных для вычисления результатов. Перед выполнением вычислений системе требуется информация по крайней мере с 5 устройств.|
|Завершена|3|Область устройства включена и завершен пересчет метрики отчета. Теперь область устройства готова к использованию.|
|unknownFutureValue|4|Значение заполнителя для будущего расширения.|




